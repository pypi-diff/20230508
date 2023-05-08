# Comparing `tmp/frontengine-0.0.8.tar.gz` & `tmp/frontengine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine-0.0.8.tar", last modified: Sat May  6 13:07:07 2023, max compression
+gzip compressed data, was "frontengine-0.0.9.tar", last modified: Sat May  6 13:56:28 2023, max compression
```

## Comparing `frontengine-0.0.8.tar` & `frontengine-0.0.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.190585 frontengine-0.0.8/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1414 2023-05-06 13:07:07.189589 frontengine-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.900360 frontengine-0.0.8/frontengine/
--rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine-0.0.8/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.951225 frontengine-0.0.8/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.955220 frontengine-0.0.8/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.958205 frontengine-0.0.8/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1451 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.966185 frontengine-0.0.8/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.8/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1441 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1648 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.970174 frontengine-0.0.8/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1443 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.981144 frontengine-0.0.8/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.008072 frontengine-0.0.8/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      825 2023-05-06 13:06:42.000000 frontengine-0.0.8/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.011065 frontengine-0.0.8/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.017050 frontengine-0.0.8/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.8/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2659 2023-05-06 12:49:14.000000 frontengine-0.0.8/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.021038 frontengine-0.0.8/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.033006 frontengine-0.0.8/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.8/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.039997 frontengine-0.0.8/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.8/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.045972 frontengine-0.0.8/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.8/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.049961 frontengine-0.0.8/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.8/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.057939 frontengine-0.0.8/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.8/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.065918 frontengine-0.0.8/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.8/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.073897 frontengine-0.0.8/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.078883 frontengine-0.0.8/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.8/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.087860 frontengine-0.0.8/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.8/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.092846 frontengine-0.0.8/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.8/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.098830 frontengine-0.0.8/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.8/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.104817 frontengine-0.0.8/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.8/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.110799 frontengine-0.0.8/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.8/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.8/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.115785 frontengine-0.0.8/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.8/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.135735 frontengine-0.0.8/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.139725 frontengine-0.0.8/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.145705 frontengine-0.0.8/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.157674 frontengine-0.0.8/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.168645 frontengine-0.0.8/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:07.185598 frontengine-0.0.8/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.8/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:07:06.948233 frontengine-0.0.8/frontengine.egg-info/
--rw-rw-rw-   0        0        0     1414 2023-05-06 13:07:06.000000 frontengine-0.0.8/frontengine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2494 2023-05-06 13:07:06.000000 frontengine-0.0.8/frontengine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:07:06.000000 frontengine-0.0.8/frontengine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 13:07:06.000000 frontengine-0.0.8/frontengine.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 13:07:06.000000 frontengine-0.0.8/frontengine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1138 2023-05-06 13:06:42.000000 frontengine-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 13:07:07.191582 frontengine-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.924368 frontengine-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1414 2023-05-06 13:56:28.923372 frontengine-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.788731 frontengine-0.0.9/frontengine/
+-rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine-0.0.9/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.824636 frontengine-0.0.9/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.827627 frontengine-0.0.9/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-05-06 13:06:42.000000 frontengine-0.0.9/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.830620 frontengine-0.0.9/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1451 2023-05-06 13:06:42.000000 frontengine-0.0.9/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.834609 frontengine-0.0.9/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.9/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1629 2023-05-06 13:44:28.000000 frontengine-0.0.9/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1797 2023-05-06 13:45:11.000000 frontengine-0.0.9/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.837601 frontengine-0.0.9/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1443 2023-05-06 13:06:42.000000 frontengine-0.0.9/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.841591 frontengine-0.0.9/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1969 2023-05-06 13:45:11.000000 frontengine-0.0.9/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.844582 frontengine-0.0.9/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-05-06 13:06:42.000000 frontengine-0.0.9/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.845579 frontengine-0.0.9/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.848572 frontengine-0.0.9/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine-0.0.9/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2659 2023-05-06 12:49:14.000000 frontengine-0.0.9/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.850566 frontengine-0.0.9/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.852561 frontengine-0.0.9/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine-0.0.9/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.856550 frontengine-0.0.9/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine-0.0.9/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.859542 frontengine-0.0.9/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine-0.0.9/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.861537 frontengine-0.0.9/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine-0.0.9/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.865527 frontengine-0.0.9/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine-0.0.9/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.868518 frontengine-0.0.9/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine-0.0.9/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.871510 frontengine-0.0.9/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.875500 frontengine-0.0.9/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine-0.0.9/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.878492 frontengine-0.0.9/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine-0.0.9/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.883478 frontengine-0.0.9/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine-0.0.9/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.887468 frontengine-0.0.9/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine-0.0.9/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.894449 frontengine-0.0.9/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine-0.0.9/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.899435 frontengine-0.0.9/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine-0.0.9/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine-0.0.9/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.900432 frontengine-0.0.9/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine-0.0.9/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.906417 frontengine-0.0.9/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.908411 frontengine-0.0.9/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.910405 frontengine-0.0.9/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.914396 frontengine-0.0.9/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.917387 frontengine-0.0.9/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.920379 frontengine-0.0.9/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine-0.0.9/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:56:28.822641 frontengine-0.0.9/frontengine.egg-info/
+-rw-rw-rw-   0        0        0     1414 2023-05-06 13:56:28.000000 frontengine-0.0.9/frontengine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2494 2023-05-06 13:56:28.000000 frontengine-0.0.9/frontengine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:56:28.000000 frontengine-0.0.9/frontengine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 13:56:28.000000 frontengine-0.0.9/frontengine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 13:56:28.000000 frontengine-0.0.9/frontengine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1138 2023-05-06 13:56:03.000000 frontengine-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 13:56:28.924368 frontengine-0.0.9/setup.cfg
```

### Comparing `frontengine-0.0.8/LICENSE` & `frontengine-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/PKG-INFO` & `frontengine-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine
-Version: 0.0.8
+Version: 0.0.9
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine-0.0.8/README.md` & `frontengine-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/show/gif/paint_gif.py` & `frontengine-0.0.9/frontengine/show/gif/paint_gif.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/show/image/paint_image.py` & `frontengine-0.0.9/frontengine/show/image/paint_image.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/show/sound_player/sound_effect.py` & `frontengine-0.0.9/frontengine/show/sound_player/sound_effect.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,16 @@
         )
         self.setAttribute(Qt.WidgetAttribute.WA_TranslucentBackground)
         self.sound_player = QSoundEffect()
         self.sound_path = Path(sound_path)
         if self.sound_path.exists() and self.sound_path.is_file():
             self.sound_player.setSource(QUrl.fromLocalFile(str(self.sound_path)))
             self.sound_player.setVolume(volume)
+            # -2 means loop forever
+            self.sound_player.setLoopCount(-2)
             self.sound_player.play()
         else:
             message_box = QMessageBox(self)
             message_box.setText("Sound file error")
             message_box.show()
         # Window setting
         self.setWindowTitle("Sound Wave")
@@ -34,7 +36,10 @@
         if self.icon_path.exists() and self.icon_path.is_file():
             self.setWindowIcon(QIcon(str(self.icon_path)))
 
     def close(self):
         super().close()
         self.sound_player.stop()
 
+    def closeEvent(self, event):
+        super().closeEvent(event)
+        self.sound_player.stop()
```

### Comparing `frontengine-0.0.8/frontengine/show/sound_player/sound_player.py` & `frontengine-0.0.9/frontengine/show/sound_player/sound_player.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         if self.sound_path.exists() and self.sound_path.is_file():
             self.media_player = QMediaPlayer()
             self.media_player_audio = QAudioOutput()
             self.media_player.setAudioOutput(self.media_player_audio)
             self.media_player_audio = self.media_player.audioOutput()
             self.media_player.setSource(QUrl.fromLocalFile(str(self.sound_path)))
             self.media_player_audio.setVolume(volume)
+            self.media_player.setLoops(-1)
             self.media_player.play()
         else:
             message_box = QMessageBox(self)
             message_box.setText("Sound file error")
             message_box.show()
         # Window setting
         self.setWindowTitle("Sound")
@@ -36,7 +37,11 @@
         self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
         if self.icon_path.exists() and self.icon_path.is_file():
             self.setWindowIcon(QIcon(str(self.icon_path)))
 
     def close(self):
         super().close()
         self.media_player.stop()
+
+    def closeEvent(self, event):
+        super().closeEvent(event)
+        self.media_player.stop()
```

### Comparing `frontengine-0.0.8/frontengine/show/text/draw_text.py` & `frontengine-0.0.9/frontengine/show/text/draw_text.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/show/video/video_player.py` & `frontengine-0.0.9/frontengine/show/video/video_player.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,20 +29,22 @@
             self.video_file_path = str(self.video_path)
             self.audioOutput = QAudioOutput()
             self.media_player.setSource(QUrl.fromLocalFile(str(self.video_file_path)))
             self.media_player.setVideoOutput(self)
             self.media_player.setAudioOutput(self.audioOutput)
             self.media_player.setPlaybackRate(play_rate)
             self.media_player.audioOutput().setVolume(volume)
+            self.media_player.setLoops(-1)
             self.media_player.play()
         else:
             message_box = QMessageBox(self)
             message_box.setText("Video error")
             message_box.show()
         self.setWindowTitle("Video")
         # Set Icon
         self.icon_path = Path(os.getcwd() + "/je_driver_icon.ico")
         if self.icon_path.exists() and self.icon_path.is_file():
             self.setWindowIcon(QIcon(str(self.icon_path)))
 
     def closeEvent(self, event):
+        super().closeEvent(event)
         self.media_player.stop()
```

### Comparing `frontengine-0.0.8/frontengine/show/web/webview.py` & `frontengine-0.0.9/frontengine/show/web/webview.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/main/main_ui.py` & `frontengine-0.0.9/frontengine/ui/main/main_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine-0.0.9/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine-0.0.9/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine-0.0.9/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine-0.0.9/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine-0.0.9/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine-0.0.9/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/utils/file/open/open_file.py` & `frontengine-0.0.9/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/utils/file/save/save_file.py` & `frontengine-0.0.9/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/utils/json/json_file.py` & `frontengine-0.0.9/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine/utils/json_format/json_process.py` & `frontengine-0.0.9/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/frontengine.egg-info/PKG-INFO` & `frontengine-0.0.9/frontengine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine
-Version: 0.0.8
+Version: 0.0.9
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine-0.0.8/frontengine.egg-info/SOURCES.txt` & `frontengine-0.0.9/frontengine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine-0.0.8/pyproject.toml` & `frontengine-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     { name = "JE-Chen", email = "jechenmailman@gmail.com" },
 ]
 dependencies = [
     "PySide6",
     "qt-material",
 ]
```

