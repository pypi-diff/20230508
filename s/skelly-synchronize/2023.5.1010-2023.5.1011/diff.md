# Comparing `tmp/skelly_synchronize-2023.5.1010.tar.gz` & `tmp/skelly_synchronize-2023.5.1011.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1010.tar", last modified: Fri May  5 19:56:55 2023, max compression
+gzip compressed data, was "skelly_synchronize-2023.5.1011.tar", last modified: Mon May  8 16:34:59 2023, max compression
```

## Comparing `skelly_synchronize-2023.5.1010.tar` & `skelly_synchronize-2023.5.1011.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       65 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/LICENSE
--rw-r--r--   0        0        0     3030 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/README.md
--rw-r--r--   0        0        0     1608 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/pyproject.toml
--rw-r--r--   0        0        0      123 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/setup.py
--rw-r--r--   0        0        0     1045 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     1961 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      821 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/debug_output.py
--rw-r--r--   0        0        0     1557 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     2699 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     4536 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1799 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     4702 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      262 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1085 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0      656 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      847 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      577 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1061 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     2317 2023-05-05 19:56:48.820764 skelly_synchronize-2023.5.1010/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1010/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/.gitattributes
+-rw-r--r--   0        0        0      146 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/.gitignore
+-rw-r--r--   0        0        0    34523 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/LICENSE
+-rw-r--r--   0        0        0     3030 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/README.md
+-rw-r--r--   0        0        0     1608 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/pyproject.toml
+-rw-r--r--   0        0        0      123 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/setup.py
+-rw-r--r--   0        0        0     1056 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     1961 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      821 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/debug_output.py
+-rw-r--r--   0        0        0     1557 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     2699 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     4536 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1821 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     4732 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      323 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1085 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0      656 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      847 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      577 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1061 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1340 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     2317 2023-05-08 16:34:53.680856 skelly_synchronize-2023.5.1011/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1011/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1010/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.5.1011/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.5.1011/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/.gitignore` & `skelly_synchronize-2023.5.1011/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/LICENSE` & `skelly_synchronize-2023.5.1011/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/README.md` & `skelly_synchronize-2023.5.1011/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/pyproject.toml` & `skelly_synchronize-2023.5.1011/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1010"
+current_version = "v2023.05.1011"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1010"
+__version__ = "v2023.05.1011"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
@@ -20,11 +20,11 @@
 
 base_package_path = Path(__file__).parent
 print(f"adding base_package_path: {base_package_path} : to sys.path")
 sys.path.insert(0, str(base_package_path))  # add parent directory to sys.path
 
 from skelly_synchronize.system.default_paths import get_log_file_path
 from skelly_synchronize.system.logging_configuration import configure_logging
-from skelly_synchronize.skelly_synchronize import synchronize_videos
+from skelly_synchronize.skelly_synchronize import synchronize_videos_from_audio
 
 
 configure_logging(log_file_path=get_log_file_path())
```

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/debug_output.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     QPushButton,
     QFileDialog,
     QMainWindow,
     QLabel,
 )
 
 from gui.widgets.run_button_widget import RunButtonWidget
-from skelly_synchronize.skelly_synchronize import synchronize_videos
+from skelly_synchronize.skelly_synchronize import synchronize_videos_from_audio
 
 
 class MainWindow(QMainWindow):
     def __init__(self):
         super().__init__()
         self._folder_path = None
 
@@ -35,15 +35,15 @@
         self.folder_path_label.setFixedHeight(15)
         self._layout.addWidget(self.folder_path_label)
 
         self.run_button = RunButtonWidget()
         self.run_button.run_button_widget.setEnabled(False)
         self._layout.addWidget(self.run_button)
         self.run_button.run_button_widget.clicked.connect(
-            lambda: synchronize_videos(self._folder_path)
+            lambda: synchronize_videos_from_audio(self._folder_path)
         )
 
     def _open_session_folder_dialog(self):
         folder_input = QFileDialog.getExistingDirectory(None, "Choose a folder")
         self._folder_path = Path(folder_input)
         self.folder_path_label.setText(
             f"Selected folder of raw videos: {self._folder_path}"
```

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/skelly_synchronize.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,21 @@
 from skelly_synchronize.tests.utilities.check_list_values_are_equal import (
     check_list_values_are_equal,
 )
 from skelly_synchronize.tests.utilities.get_number_of_frames_of_videos_in_a_folder import (
     get_number_of_frames_of_videos_in_a_folder,
 )
 from skelly_synchronize.system.paths_and_file_names import (
+    DEBUG_TOML_NAME,
     SYNCHRONIZED_VIDEOS_FOLDER_NAME,
     AUDIO_FILES_FOLDER_NAME,
 )
 
 
-def synchronize_videos(
+def synchronize_videos_from_audio(
     raw_video_folder_path: Path,
     file_type: str = ".mp4",
     video_handler: str = "deffcode",
 ):
     """Run the functions from the VideoSynchronize class to synchronize all videos with the given file type in the base path folder.
     Uses deffcode and to handle the video files as default, set "video_handler" to "ffmpeg" to use ffmpeg methods instead.
     ffmpeg is used to get audio from the video files with either method.
@@ -110,15 +111,15 @@
             "Raw video information": video_info_dict,
             "Synchronized video information": synchronized_video_info_dict,
             "Audio information": remove_audio_files_from_audio_signal_dict(
                 audio_signal_dictionary=audio_signal_dict
             ),
             "Lag dictionary": lag_dict,
         },
-        output_file_path=session_folder_path / "synchronization_debug.toml",
+        output_file_path=session_folder_path / DEBUG_TOML_NAME,
     )
 
     # end performance timer
     end_timer = time.time()
 
     # calculate and display elapsed processing time
     elapsed_time = end_timer - start_timer
@@ -126,8 +127,8 @@
 
     return synchronized_video_folder_path
 
 
 if __name__ == "__main__":
     raw_video_folder_path = Path("path/to/your/folder/of/raw/videos")
     file_type = "MP4"
-    synchronize_videos(raw_video_folder_path=raw_video_folder_path, file_type=file_type)
+    synchronize_videos_from_audio(raw_video_folder_path=raw_video_folder_path, file_type=file_type)
```

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.5.1011/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1010/PKG-INFO` & `skelly_synchronize-2023.5.1011/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1010
+Version: 2023.5.1011
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

