# Comparing `tmp/frontengine_dev-0.0.8.tar.gz` & `tmp/frontengine_dev-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frontengine_dev-0.0.8.tar", last modified: Sat May  6 13:09:26 2023, max compression
+gzip compressed data, was "frontengine_dev-0.0.9.tar", last modified: Sat May  6 13:59:18 2023, max compression
```

## Comparing `frontengine_dev-0.0.8.tar` & `frontengine_dev-0.0.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.962111 frontengine_dev-0.0.8/
--rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine_dev-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     1418 2023-05-06 13:09:26.961114 frontengine_dev-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine_dev-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.451450 frontengine_dev-0.0.8/frontengine/
--rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine_dev-0.0.8/frontengine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.453444 frontengine_dev-0.0.8/frontengine/show/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/show/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.457433 frontengine_dev-0.0.8/frontengine/show/gif/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/show/gif/__init__.py
--rw-rw-rw-   0        0        0     1882 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/gif/paint_gif.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.462421 frontengine_dev-0.0.8/frontengine/show/image/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/show/image/__init__.py
--rw-rw-rw-   0        0        0     1451 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/image/paint_image.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.470401 frontengine_dev-0.0.8/frontengine/show/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.8/frontengine/show/sound_player/__init__.py
--rw-rw-rw-   0        0        0     1441 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/sound_player/sound_effect.py
--rw-rw-rw-   0        0        0     1648 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/sound_player/sound_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.475384 frontengine_dev-0.0.8/frontengine/show/text/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/show/text/__init__.py
--rw-rw-rw-   0        0        0     1443 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/text/draw_text.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.489347 frontengine_dev-0.0.8/frontengine/show/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/show/video/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/video/video_player.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.496328 frontengine_dev-0.0.8/frontengine/show/web/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/show/web/__init__.py
--rw-rw-rw-   0        0        0      825 2023-05-06 13:06:42.000000 frontengine_dev-0.0.8/frontengine/show/web/webview.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.503309 frontengine_dev-0.0.8/frontengine/ui/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.620996 frontengine_dev-0.0.8/frontengine/ui/main/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.8/frontengine/ui/main/__init__.py
--rw-rw-rw-   0        0        0     2659 2023-05-06 12:49:14.000000 frontengine_dev-0.0.8/frontengine/ui/main/main_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.633961 frontengine_dev-0.0.8/frontengine/ui/setting/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.677357 frontengine_dev-0.0.8/frontengine/ui/setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/gif/__init__.py
--rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine_dev-0.0.8/frontengine/ui/setting/gif/gif_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.717251 frontengine_dev-0.0.8/frontengine/ui/setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/image/__init__.py
--rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine_dev-0.0.8/frontengine/ui/setting/image/image_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.739193 frontengine_dev-0.0.8/frontengine/ui/setting/sound_player/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/sound_player/__init__.py
--rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine_dev-0.0.8/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.758657 frontengine_dev-0.0.8/frontengine/ui/setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/text/__init__.py
--rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine_dev-0.0.8/frontengine/ui/setting/text/text_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.767631 frontengine_dev-0.0.8/frontengine/ui/setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/video/__init__.py
--rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine_dev-0.0.8/frontengine/ui/setting/video/video_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.779598 frontengine_dev-0.0.8/frontengine/ui/setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/ui/setting/web/__init__.py
--rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine_dev-0.0.8/frontengine/ui/setting/web/web_setting_ui.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.785583 frontengine_dev-0.0.8/frontengine/user_setting/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.801541 frontengine_dev-0.0.8/frontengine/user_setting/gif/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/gif/__init__.py
--rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine_dev-0.0.8/frontengine/user_setting/gif/gif_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.825478 frontengine_dev-0.0.8/frontengine/user_setting/image/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/image/__init__.py
--rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine_dev-0.0.8/frontengine/user_setting/image/image_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.832457 frontengine_dev-0.0.8/frontengine/user_setting/sound/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/sound/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine_dev-0.0.8/frontengine/user_setting/sound/sound_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.838442 frontengine_dev-0.0.8/frontengine/user_setting/text/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/text/__init__.py
--rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine_dev-0.0.8/frontengine/user_setting/text/text_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.846419 frontengine_dev-0.0.8/frontengine/user_setting/video/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/video/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine_dev-0.0.8/frontengine/user_setting/video/video_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.856394 frontengine_dev-0.0.8/frontengine/user_setting/web/
--rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.8/frontengine/user_setting/web/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine_dev-0.0.8/frontengine/user_setting/web/web_setting.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.860384 frontengine_dev-0.0.8/frontengine/utils/
--rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.8/frontengine/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.877338 frontengine_dev-0.0.8/frontengine/utils/exception/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/exception/__init__.py
--rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.885321 frontengine_dev-0.0.8/frontengine/utils/file/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/file/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.892303 frontengine_dev-0.0.8/frontengine/utils/file/open/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/file/open/__init__.py
--rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/file/open/open_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.897284 frontengine_dev-0.0.8/frontengine/utils/file/save/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/file/save/__init__.py
--rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/file/save/save_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.911247 frontengine_dev-0.0.8/frontengine/utils/json/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/json/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/json/json_file.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.920225 frontengine_dev-0.0.8/frontengine/utils/json_format/
--rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/json_format/__init__.py
--rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine_dev-0.0.8/frontengine/utils/json_format/json_process.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:09:26.959120 frontengine_dev-0.0.8/frontengine_dev.egg-info/
--rw-rw-rw-   0        0        0     1418 2023-05-06 13:09:26.000000 frontengine_dev-0.0.8/frontengine_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2514 2023-05-06 13:09:26.000000 frontengine_dev-0.0.8/frontengine_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:09:26.000000 frontengine_dev-0.0.8/frontengine_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 13:09:26.000000 frontengine_dev-0.0.8/frontengine_dev.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 13:09:26.000000 frontengine_dev-0.0.8/frontengine_dev.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1142 2023-05-06 13:09:04.000000 frontengine_dev-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 13:09:26.962111 frontengine_dev-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.361647 frontengine_dev-0.0.9/
+-rw-rw-rw-   0        0        0     1084 2023-04-30 07:06:10.000000 frontengine_dev-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1418 2023-05-06 13:59:18.360650 frontengine_dev-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      617 2023-05-06 09:57:23.000000 frontengine_dev-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.236981 frontengine_dev-0.0.9/frontengine/
+-rw-rw-rw-   0        0        0      104 2023-05-06 11:03:04.000000 frontengine_dev-0.0.9/frontengine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.238977 frontengine_dev-0.0.9/frontengine/show/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/show/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.241967 frontengine_dev-0.0.9/frontengine/show/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/show/gif/__init__.py
+-rw-rw-rw-   0        0        0     1882 2023-05-06 13:06:42.000000 frontengine_dev-0.0.9/frontengine/show/gif/paint_gif.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.244964 frontengine_dev-0.0.9/frontengine/show/image/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/show/image/__init__.py
+-rw-rw-rw-   0        0        0     1451 2023-05-06 13:06:42.000000 frontengine_dev-0.0.9/frontengine/show/image/paint_image.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.248949 frontengine_dev-0.0.9/frontengine/show/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.9/frontengine/show/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     1629 2023-05-06 13:44:28.000000 frontengine_dev-0.0.9/frontengine/show/sound_player/sound_effect.py
+-rw-rw-rw-   0        0        0     1797 2023-05-06 13:45:11.000000 frontengine_dev-0.0.9/frontengine/show/sound_player/sound_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.251941 frontengine_dev-0.0.9/frontengine/show/text/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/show/text/__init__.py
+-rw-rw-rw-   0        0        0     1443 2023-05-06 13:06:42.000000 frontengine_dev-0.0.9/frontengine/show/text/draw_text.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.253935 frontengine_dev-0.0.9/frontengine/show/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/show/video/__init__.py
+-rw-rw-rw-   0        0        0     1969 2023-05-06 13:45:11.000000 frontengine_dev-0.0.9/frontengine/show/video/video_player.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.256927 frontengine_dev-0.0.9/frontengine/show/web/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/show/web/__init__.py
+-rw-rw-rw-   0        0        0      825 2023-05-06 13:06:42.000000 frontengine_dev-0.0.9/frontengine/show/web/webview.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.257925 frontengine_dev-0.0.9/frontengine/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.260917 frontengine_dev-0.0.9/frontengine/ui/main/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:26.000000 frontengine_dev-0.0.9/frontengine/ui/main/__init__.py
+-rw-rw-rw-   0        0        0     2659 2023-05-06 12:49:14.000000 frontengine_dev-0.0.9/frontengine/ui/main/main_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.261914 frontengine_dev-0.0.9/frontengine/ui/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.264907 frontengine_dev-0.0.9/frontengine/ui/setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/gif/__init__.py
+-rw-rw-rw-   0        0        0     4494 2023-05-05 19:12:06.000000 frontengine_dev-0.0.9/frontengine/ui/setting/gif/gif_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.267898 frontengine_dev-0.0.9/frontengine/ui/setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/image/__init__.py
+-rw-rw-rw-   0        0        0     3713 2023-05-06 06:45:53.000000 frontengine_dev-0.0.9/frontengine/ui/setting/image/image_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.271890 frontengine_dev-0.0.9/frontengine/ui/setting/sound_player/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/sound_player/__init__.py
+-rw-rw-rw-   0        0        0     6034 2023-05-06 06:47:02.000000 frontengine_dev-0.0.9/frontengine/ui/setting/sound_player/sound_player_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.276874 frontengine_dev-0.0.9/frontengine/ui/setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/text/__init__.py
+-rw-rw-rw-   0        0        0     2958 2023-05-06 05:39:36.000000 frontengine_dev-0.0.9/frontengine/ui/setting/text/text_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.280863 frontengine_dev-0.0.9/frontengine/ui/setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/video/__init__.py
+-rw-rw-rw-   0        0        0     5385 2023-05-06 06:40:18.000000 frontengine_dev-0.0.9/frontengine/ui/setting/video/video_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.286848 frontengine_dev-0.0.9/frontengine/ui/setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/ui/setting/web/__init__.py
+-rw-rw-rw-   0        0        0     1949 2023-05-06 06:03:35.000000 frontengine_dev-0.0.9/frontengine/ui/setting/web/web_setting_ui.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.288843 frontengine_dev-0.0.9/frontengine/user_setting/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.291834 frontengine_dev-0.0.9/frontengine/user_setting/gif/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/gif/__init__.py
+-rw-rw-rw-   0        0        0       89 2023-05-05 14:57:05.000000 frontengine_dev-0.0.9/frontengine/user_setting/gif/gif_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.295824 frontengine_dev-0.0.9/frontengine/user_setting/image/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/image/__init__.py
+-rw-rw-rw-   0        0        0       79 2023-05-05 12:53:50.000000 frontengine_dev-0.0.9/frontengine/user_setting/image/image_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.298815 frontengine_dev-0.0.9/frontengine/user_setting/sound/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/sound/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:36:27.000000 frontengine_dev-0.0.9/frontengine/user_setting/sound/sound_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.303805 frontengine_dev-0.0.9/frontengine/user_setting/text/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/text/__init__.py
+-rw-rw-rw-   0        0        0       98 2023-05-05 13:01:58.000000 frontengine_dev-0.0.9/frontengine/user_setting/text/text_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.307792 frontengine_dev-0.0.9/frontengine/user_setting/video/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/video/__init__.py
+-rw-rw-rw-   0        0        0      118 2023-05-05 13:59:59.000000 frontengine_dev-0.0.9/frontengine/user_setting/video/video_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.310783 frontengine_dev-0.0.9/frontengine/user_setting/web/
+-rw-rw-rw-   0        0        0        0 2023-05-04 11:53:07.000000 frontengine_dev-0.0.9/frontengine/user_setting/web/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-05 13:03:17.000000 frontengine_dev-0.0.9/frontengine/user_setting/web/web_setting.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.312778 frontengine_dev-0.0.9/frontengine/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-02 10:51:49.000000 frontengine_dev-0.0.9/frontengine/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.317765 frontengine_dev-0.0.9/frontengine/utils/exception/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0      248 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      236 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.319760 frontengine_dev-0.0.9/frontengine/utils/file/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/file/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.323749 frontengine_dev-0.0.9/frontengine/utils/file/open/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/file/open/__init__.py
+-rw-rw-rw-   0        0        0      976 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/file/open/open_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.326742 frontengine_dev-0.0.9/frontengine/utils/file/save/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/file/save/__init__.py
+-rw-rw-rw-   0        0        0      733 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/file/save/save_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.330731 frontengine_dev-0.0.9/frontengine/utils/json/
+-rw-rw-rw-   0        0        0        0 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/json/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/json/json_file.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.333722 frontengine_dev-0.0.9/frontengine/utils/json_format/
+-rw-rw-rw-   0        0        0        2 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/json_format/__init__.py
+-rw-rw-rw-   0        0        0     1021 2023-05-05 11:00:27.000000 frontengine_dev-0.0.9/frontengine/utils/json_format/json_process.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:59:18.358657 frontengine_dev-0.0.9/frontengine_dev.egg-info/
+-rw-rw-rw-   0        0        0     1418 2023-05-06 13:59:18.000000 frontengine_dev-0.0.9/frontengine_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2514 2023-05-06 13:59:18.000000 frontengine_dev-0.0.9/frontengine_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:59:18.000000 frontengine_dev-0.0.9/frontengine_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-06 13:59:18.000000 frontengine_dev-0.0.9/frontengine_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-06 13:59:18.000000 frontengine_dev-0.0.9/frontengine_dev.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1142 2023-05-06 13:59:01.000000 frontengine_dev-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 13:59:18.361647 frontengine_dev-0.0.9/setup.cfg
```

### Comparing `frontengine_dev-0.0.8/LICENSE` & `frontengine_dev-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/PKG-INFO` & `frontengine_dev-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine_dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine_dev-0.0.8/README.md` & `frontengine_dev-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/show/gif/paint_gif.py` & `frontengine_dev-0.0.9/frontengine/show/gif/paint_gif.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/show/image/paint_image.py` & `frontengine_dev-0.0.9/frontengine/show/image/paint_image.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/show/sound_player/sound_effect.py` & `frontengine_dev-0.0.9/frontengine/show/sound_player/sound_effect.py`

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

### Comparing `frontengine_dev-0.0.8/frontengine/show/sound_player/sound_player.py` & `frontengine_dev-0.0.9/frontengine/show/sound_player/sound_player.py`

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

### Comparing `frontengine_dev-0.0.8/frontengine/show/text/draw_text.py` & `frontengine_dev-0.0.9/frontengine/show/text/draw_text.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/show/video/video_player.py` & `frontengine_dev-0.0.9/frontengine/show/video/video_player.py`

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

### Comparing `frontengine_dev-0.0.8/frontengine/show/web/webview.py` & `frontengine_dev-0.0.9/frontengine/show/web/webview.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/main/main_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/main/main_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/setting/gif/gif_setting_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/setting/gif/gif_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/setting/image/image_setting_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/setting/image/image_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/setting/sound_player/sound_player_setting_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/setting/sound_player/sound_player_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/setting/text/text_setting_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/setting/text/text_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/setting/video/video_setting_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/setting/video/video_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/ui/setting/web/web_setting_ui.py` & `frontengine_dev-0.0.9/frontengine/ui/setting/web/web_setting_ui.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/utils/file/open/open_file.py` & `frontengine_dev-0.0.9/frontengine/utils/file/open/open_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/utils/file/save/save_file.py` & `frontengine_dev-0.0.9/frontengine/utils/file/save/save_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/utils/json/json_file.py` & `frontengine_dev-0.0.9/frontengine/utils/json/json_file.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine/utils/json_format/json_process.py` & `frontengine_dev-0.0.9/frontengine/utils/json_format/json_process.py`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/frontengine_dev.egg-info/PKG-INFO` & `frontengine_dev-0.0.9/frontengine_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frontengine-dev
-Version: 0.0.8
+Version: 0.0.9
 Summary: FrontEngine is a tool allow you set Video or Image or GIF front of all window
 Author-email: JE-Chen <jechenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Intergration-Automation-Testing/FrontEngine
 Project-URL: Code, https://github.com/Intergration-Automation-Testing/FrontEngine
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `frontengine_dev-0.0.8/frontengine_dev.egg-info/SOURCES.txt` & `frontengine_dev-0.0.9/frontengine_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frontengine_dev-0.0.8/pyproject.toml` & `frontengine_dev-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "frontengine_dev"
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

