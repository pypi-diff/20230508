# Comparing `tmp/skelly_viewer-2023.3.1017.tar.gz` & `tmp/skelly_viewer-2023.5.1018.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_viewer-2023.3.1017.tar", last modified: Sat Mar 11 16:58:57 2023, max compression
+gzip compressed data, was "skelly_viewer-2023.5.1018.tar", last modified: Mon May  8 20:24:18 2023, max compression
```

## Comparing `skelly_viewer-2023.3.1017.tar` & `skelly_viewer-2023.5.1018.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       66 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/.gitattributes
--rw-r--r--   0        0        0     1087 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     2784 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/.gitignore
--rw-r--r--   0        0        0     1067 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/LICENSE
--rw-r--r--   0        0        0      989 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/README.md
--rw-r--r--   0        0        0     1660 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/pyproject.toml
--rw-r--r--   0        0        0       50 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/setup.py
--rw-r--r--   0        0        0     1023 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/__init__.py
--rw-r--r--   0        0        0      351 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/__main__.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/config/__init__.py
--rw-r--r--   0        0        0     1382 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/config/default_paths.py
--rw-r--r--   0        0        0      478 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/config/folder_and_file_names.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/config/init.py
--rw-r--r--   0        0        0     1406 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/config/logging_configuration.py
--rw-r--r--   0        0        0     1554 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/experimental/checkable_combo_box.py
--rw-r--r--   0        0        0     1155 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/__init__.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/__init__.py
--rw-r--r--   0        0        0     3135 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/skelly_viewer_widget.py
--rw-r--r--   0        0        0     2963 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/skellyview_main_window.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/init.py
--rw-r--r--   0        0        0     4057 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/multi_video_display.py
--rw-r--r--   0        0        0     4661 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py
--rw-r--r--   0        0        0     3247 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/slider_widget.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/__init__.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/__init__.py
--rw-r--r--   0        0        0      965 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py
--rw-r--r--   0        0        0     1896 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py
--rw-r--r--   0        0        0     2168 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py
--rw-r--r--   0        0        0      134 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/test_test.py
--rw-r--r--   0        0        0        0 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/utilities/__init__.py
--rw-r--r--   0        0        0     2329 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/utilities/freemocap_data_loader.py
--rw-r--r--   0        0        0      850 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/utilities/load_sample_data.py
--rw-r--r--   0        0        0     6077 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/utilities/mediapipe_skeleton_builder.py
--rw-r--r--   0        0        0     1805 2023-03-11 16:58:52.942172 skelly_viewer-2023.3.1017/skelly_viewer/utilities/video_handler.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 skelly_viewer-2023.3.1017/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-05-08 20:24:10.153940 skelly_viewer-2023.5.1018/.gitattributes
+-rw-r--r--   0        0        0     1087 2023-05-08 20:24:10.153940 skelly_viewer-2023.5.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     2784 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/.gitignore
+-rw-r--r--   0        0        0     1067 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/LICENSE
+-rw-r--r--   0        0        0      989 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/README.md
+-rw-r--r--   0        0        0     1660 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/setup.py
+-rw-r--r--   0        0        0     1023 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/__init__.py
+-rw-r--r--   0        0        0      351 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/__init__.py
+-rw-r--r--   0        0        0     1382 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/default_paths.py
+-rw-r--r--   0        0        0      478 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/folder_and_file_names.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/init.py
+-rw-r--r--   0        0        0     1406 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/config/logging_configuration.py
+-rw-r--r--   0        0        0     1554 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/experimental/checkable_combo_box.py
+-rw-r--r--   0        0        0     1155 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/__init__.py
+-rw-r--r--   0        0        0     3418 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skelly_viewer_widget.py
+-rw-r--r--   0        0        0     2945 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skellyview_main_window.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/init.py
+-rw-r--r--   0        0        0     5825 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/multi_video_display.py
+-rw-r--r--   0        0        0     6284 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py
+-rw-r--r--   0        0        0     2648 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/slider_widget.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/__init__.py
+-rw-r--r--   0        0        0      965 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py
+-rw-r--r--   0        0        0     1896 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py
+-rw-r--r--   0        0        0     2168 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py
+-rw-r--r--   0        0        0      134 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/test_test.py
+-rw-r--r--   0        0        0        0 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/__init__.py
+-rw-r--r--   0        0        0     2329 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/freemocap_data_loader.py
+-rw-r--r--   0        0        0      850 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     6077 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/mediapipe_skeleton_builder.py
+-rw-r--r--   0        0        0     1805 2023-05-08 20:24:10.157940 skelly_viewer-2023.5.1018/skelly_viewer/utilities/video_handler.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 skelly_viewer-2023.5.1018/PKG-INFO
```

### Comparing `skelly_viewer-2023.3.1017/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_viewer-2023.5.1018/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/.gitignore` & `skelly_viewer-2023.5.1018/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/LICENSE` & `skelly_viewer-2023.5.1018/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/README.md` & `skelly_viewer-2023.5.1018/README.md`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/pyproject.toml` & `skelly_viewer-2023.5.1018/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.03.1017"
+current_version = "v2023.05.1018"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/__init__.py` & `skelly_viewer-2023.5.1018/skelly_viewer/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_viewer"
-__version__ = "v2023.03.1017"
+__version__ = "v2023.05.1018"
 
 __author__ = """Skelly FreeMoCap"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 __repo_issues_url__ = f"{__repo_url__}issues"
```

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/config/default_paths.py` & `skelly_viewer-2023.5.1018/skelly_viewer/config/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/config/logging_configuration.py` & `skelly_viewer-2023.5.1018/skelly_viewer/config/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/experimental/checkable_combo_box.py` & `skelly_viewer-2023.5.1018/skelly_viewer/experimental/checkable_combo_box.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py` & `skelly_viewer-2023.5.1018/skelly_viewer/experimental/plotly/plotly_gpt_anim_working1.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/skelly_viewer_widget.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skelly_viewer_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
         self._frame_count_slider = PlayPauseCountSlider()
         self._frame_count_slider.setEnabled(False)
         layout.addWidget(self._frame_count_slider)
 
         self.connect_signals_to_slots()
 
+        self._is_video_display_enabled = True
+
         if mediapipe_skeleton_npy_path is not None:
             self.load_skeleton_data(mediapipe_skeleton_npy_path)
 
         if video_folder_path is not None:
             self.generate_video_display(video_folder_path)
 
     def load_skeleton_data(self, mediapipe_skeleton_npy_path: Union[str, Path]):
@@ -66,8 +68,13 @@
 
     def _handle_data_loaded_signal(self):
         self._frame_count_slider.set_slider_range(self._skeleton_view_widget._number_of_frames)
         self._frame_count_slider.setEnabled(True)
 
     def _handle_slider_value_changed(self):
         self._skeleton_view_widget.update_skeleton_plot(self._frame_count_slider._slider.value())
-        self.multi_video_display.update_display(self._frame_count_slider._slider.value())
+        if self._is_video_display_enabled:
+            self.multi_video_display.update_display(self._frame_count_slider._slider.value())
+
+    def toggle_video_display(self):
+        self._is_video_display_enabled = not self._is_video_display_enabled
+        self.multi_video_display.setVisible(self._is_video_display_enabled)
```

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/skellyview_main_window.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/skellyview_main_window.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import zipfile
 from pathlib import Path
 from typing import Union
 
 from PyQt6.QtWidgets import QApplication, QWidget, QVBoxLayout, QPushButton, QFileDialog, QMainWindow, QHBoxLayout
 
 from skelly_viewer import SkellyViewer
-import requests
-import io
 
 from skelly_viewer.config.folder_and_file_names import BASE_FOLDER_NAME, SAMPLE_DATA_FILE_NAME, \
     MEDIAPIPE_3D_BODY_FILE_NAME, OUTPUT_DATA_FOLDER_NAME
 from skelly_viewer.utilities.freemocap_data_loader import FreeMoCapDataLoader
 from skelly_viewer.utilities.load_sample_data import load_sample_data
 
 
@@ -20,35 +17,35 @@
         self.setWindowTitle('Skelly Viewer \U0001F480 \U0001F440')
         self.setGeometry(100, 100, 1200, 600)
         widget = QWidget()
         self._layout = QVBoxLayout()
         widget.setLayout(self._layout)
         self.setCentralWidget(widget)
 
+        hbox = QHBoxLayout()
+        self._layout.addLayout(hbox)
+
         self._folder_open_button = QPushButton('Load a session folder', self)
         self._folder_open_button.clicked.connect(self._open_session_folder_dialog)
+        hbox.addWidget(self._folder_open_button)
 
         self._sample_data_loader_button = QPushButton('Load sample data', self)
         self._sample_data_loader_button.clicked.connect(lambda: self._load_data(path=load_sample_data()))
-        self._layout.addWidget(self._sample_data_loader_button)
-
-        # self._video_folder_load_button = QPushButton('Load a folder of videos', self)
-        # self._video_folder_load_button.setEnabled(False)
-        # self._video_folder_load_button.clicked.connect(self.open_video_folder_dialogue)
-
-        hbox = QHBoxLayout()
-        hbox.addWidget(self._folder_open_button)
-        # hbox.addWidget(self._video_folder_load_button)
-        self._layout.addLayout(hbox)
-
+        hbox.addWidget(self._sample_data_loader_button)
 
+        self._toggle_video_display_button = QPushButton('Toggle Video Display', self)
+        self._toggle_video_display_button.clicked.connect(self._toggle_video_display)
+        hbox.addWidget(self._toggle_video_display_button)
 
         self._skelly_viewer = SkellyViewer()
         self._layout.addWidget(self._skelly_viewer)
 
+    def _toggle_video_display(self):
+        self._skelly_viewer.toggle_video_display()
+        
     def _open_session_folder_dialog(self):
         folder_path = QFileDialog.getExistingDirectory(None, "Choose a FreeMoCap recording folder",)
 
         if folder_path:
             self._load_data(path=folder_path)
 
     # def open_video_folder_dialogue(self):
```

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/skeleton_view_widget.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 from typing import Union
-
-
 from PyQt6.QtCore import pyqtSignal
 from PyQt6.QtWidgets import QWidget, QVBoxLayout
-
 from skelly_viewer.utilities.mediapipe_skeleton_builder import build_skeleton, mediapipe_indices, mediapipe_connections
-
-
 import matplotlib
-
 matplotlib.use('Qt5Agg')
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 from matplotlib.figure import Figure
-
 from pathlib import Path
 import numpy as np
 
-
 class SkeletonViewWidget(QWidget):
     skeleton_data_loaded_signal = pyqtSignal()
 
     def __init__(self):
         super().__init__()
 
         self._layout = QVBoxLayout()
         self.setLayout(self._layout)
 
         self._figure_widget, self._3d_axes = self.initialize_skeleton_plot()
         self._layout.addWidget(self._figure_widget)
+        self._skel_bones = None
 
     def load_skeleton_data(self, mediapipe_skeleton_npy_path: Union[str, Path]):
         self._skeleton_3d_frame_marker_xyz = np.load(str(mediapipe_skeleton_npy_path))
         self._mediapipe_skeleton = build_skeleton(skeleton_3d_frame_marker_xyz=self._skeleton_3d_frame_marker_xyz,
                                                   pose_estimation_markers_list=mediapipe_indices,
                                                   pose_estimation_connections_dict=mediapipe_connections)
 
@@ -46,64 +39,90 @@
         axes = figure_widget.figure.axes[0]
         return figure_widget, axes
 
     def _initialize_3d_axes(self):
         self._3d_axes.cla()
         self._calculate_axes_means(self._skeleton_3d_frame_marker_xyz)
         self.skel_x, self.skel_y, self.skel_z = self._get_x_y_z_data(0)
-        self._plot_skeleton(0, self.skel_x, self.skel_y, self.skel_z)
+        self.skel_points = self._3d_axes.scatter(self.skel_x, self.skel_y, self.skel_z, 'ko', s=1)
+        self.skel_bones = self._plot_skeleton_bones(0)
 
     def reset_slider(self):
         self._slider_max = self._number_of_frames - 1
         self.slider.setValue(0)
         self.slider.setMaximum(self._slider_max)
 
     def _calculate_axes_means(self, skeleton_3d_frame_marker_xyz: np.ndarray):
         self._data_midpoint_x = np.nanmean(skeleton_3d_frame_marker_xyz[:, :, 0])
         self._data_midpoint_y = np.nanmean(skeleton_3d_frame_marker_xyz[:, :, 1])
         self._data_midpoint_z = np.nanmean(skeleton_3d_frame_marker_xyz[:, :, 2])
         self._axes_3d_range = 1000
 
     def _plot_skeleton(self, frame_number, skeleton_points_x, skeleton_points_y, skeleton_points_z):
-        self._3d_axes.scatter(skeleton_points_x, skeleton_points_y, skeleton_points_z, 'ko', s=1)
+        
+        self.skel_points.set_offsets(np.column_stack([skeleton_points_x, skeleton_points_y]))
+        self.skel_points.set_3d_properties(skeleton_points_z, zdir='z')
         self._plot_skeleton_bones(frame_number)
+
         self._3d_axes.set_xlim(
-            [self._data_midpoint_x - self._axes_3d_range, self._data_midpoint_x + self._axes_3d_range])
+        [self._data_midpoint_x - self._axes_3d_range, self._data_midpoint_x + self._axes_3d_range])
         self._3d_axes.set_ylim(
-            [self._data_midpoint_y - self._axes_3d_range, self._data_midpoint_y + self._axes_3d_range])
+        [self._data_midpoint_y - self._axes_3d_range, self._data_midpoint_y + self._axes_3d_range])
         self._3d_axes.set_zlim(
-            [self._data_midpoint_z - self._axes_3d_range, self._data_midpoint_z + self._axes_3d_range])
+        [self._data_midpoint_z - self._axes_3d_range, self._data_midpoint_z + self._axes_3d_range])
 
         self._figure_widget.figure.canvas.draw_idle()
 
     def _plot_skeleton_bones(self, frame_number):
-        this_frame_skeleton_data = self._mediapipe_skeleton[frame_number]
-        for connection in this_frame_skeleton_data.keys():
-            line_start_point = this_frame_skeleton_data[connection][0]
-            line_end_point = this_frame_skeleton_data[connection][1]
-
-            bone_x, bone_y, bone_z = [line_start_point[0], line_end_point[0]], [line_start_point[1],
-                                                                                line_end_point[1]], [
-                                         line_start_point[2], line_end_point[2]]
+        if self._skel_bones is None:
+            this_frame_skeleton_data = self._mediapipe_skeleton[frame_number]
+            self._skel_bones = []
+            for connection in this_frame_skeleton_data.keys():
+                line_start_point = this_frame_skeleton_data[connection][0]
+                line_end_point = this_frame_skeleton_data[connection][1]
+
+                bone_x, bone_y, bone_z = [line_start_point[0], line_end_point[0]], [line_start_point[1],
+                                                                                    line_end_point[1]], [
+                                             line_start_point[2], line_end_point[2]]
+                bone = self._3d_axes.plot(bone_x, bone_y, bone_z)[0]
+                self._skel_bones.append(bone)
+        else:
+            this_frame_skeleton_data = self._mediapipe_skeleton[frame_number]
+            for i, connection in enumerate(this_frame_skeleton_data.keys()):
+                line_start_point = this_frame_skeleton_data[connection][0]
+                line_end_point = this_frame_skeleton_data[connection][1]
+
+                bone_x, bone_y, bone_z = [line_start_point[0], line_end_point[0]], [line_start_point[1],
+                                                                                    line_end_point[1]], [
+                                             line_start_point[2], line_end_point[2]]
+                bone = self._skel_bones[i]
+                bone.set_xdata(bone_x)
+                bone.set_ydata(bone_y)
+                bone.set_3d_properties(bone_z)
 
-            self._3d_axes.plot(bone_x, bone_y, bone_z)
 
     def _get_x_y_z_data(self, frame_number: int):
+        
         skel_x = self._skeleton_3d_frame_marker_xyz[frame_number, :, 0]
         skel_y = self._skeleton_3d_frame_marker_xyz[frame_number, :, 1]
         skel_z = self._skeleton_3d_frame_marker_xyz[frame_number, :, 2]
 
         return skel_x, skel_y, skel_z
 
     def update_skeleton_plot(self, frame_number: int):
         skel_x, skel_y, skel_z = self._get_x_y_z_data(frame_number)
-        self._3d_axes.cla()
-        self._plot_skeleton(frame_number, skel_x, skel_y, skel_z)
-        # self.label.setText(str(frame_number))
-
+        self.skel_points.set_offsets(np.column_stack([skel_x, skel_y]))
+        self.skel_points.set_3d_properties(skel_z, zdir='z')
+        self._plot_skeleton_bones(frame_number)
+        self._3d_axes.set_xlim(
+            [self._data_midpoint_x - self._axes_3d_range, self._data_midpoint_x + self._axes_3d_range])
+        self._3d_axes.set_ylim(
+            [self._data_midpoint_y - self._axes_3d_range, self._data_midpoint_y + self._axes_3d_range])
+        self._3d_axes.set_zlim(
+            [self._data_midpoint_z - self._axes_3d_range, self._data_midpoint_z + self._axes_3d_range])
+        self._figure_widget.figure.canvas.draw_idle()
 
 class Mpl3DPlotCanvas(FigureCanvasQTAgg):
-
     def __init__(self, parent=None, width=4, height=4, dpi=100):
         fig = Figure(figsize=(width, height), dpi=dpi)
         self.axes = fig.add_subplot(111, projection='3d')
         super(Mpl3DPlotCanvas, self).__init__(fig)
```

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/slider_widget.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/slider_widget.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,102 +1,86 @@
 from PyQt6.QtCore import Qt, QTimer, pyqtSlot
 from PyQt6.QtWidgets import QSlider, QWidget, QLabel, QHBoxLayout, QPushButton, QVBoxLayout
 
 PRESUMED_FRAMES_PER_SECOND = 30
 
+
 class QSliderButton(QPushButton):
     def __init__(self, text):
         super().__init__(text)
         self.setFixedWidth(75)
 
+
 class PlayPauseCountSlider(QWidget):
     def __init__(self):
         super().__init__()
 
         self._timer = QTimer()
         self._timer.timeout.connect(self._timer_timeout)
 
-        self._layout = QVBoxLayout()
-        self.setLayout(self._layout)
+        self._layout = QVBoxLayout(self)
 
         slider_hbox = QHBoxLayout()
         self._layout.addLayout(slider_hbox)
 
         self._slider = QSlider(Qt.Orientation.Horizontal)
         slider_hbox.addWidget(self._slider)
-        self._slider.setMaximum(0)
-        self._slider.valueChanged.connect(lambda: self._frame_count_label.setText(str(self._slider.value())))
+        self.slider_max = 0
+        self._slider.valueChanged.connect(lambda: self._frame_count_label.setText(f"Frame# {self._slider.value()}"))
 
         self._frame_count_label = QLabel(f"Frame# {self._slider.value()}")
-
         slider_hbox.addWidget(self._frame_count_label)
 
-
         hbox = QHBoxLayout()
         self._layout.addLayout(hbox)
 
         self._play_button = QSliderButton("Play")
         self._play_button.clicked.connect(self._play_button_clicked)
         hbox.addWidget(self._play_button)
-        #
-        # self._play_double_speed_button = QSliderButton("Play x2")
-        # self._play_button.clicked.connect(self._play_double_speed_button_clicked)
-        # hbox.addWidget(self._play_double_speed_button)
-        #
-        # self._play_half_speed_button = QSliderButton("Play x1/2")
-        # self._play_button.clicked.connect(self._play_half_speed_button_clicked)
-        # hbox.addWidget(self._play_half_speed_button)
 
         self._pause_button = QSliderButton("Pause")
         self._pause_button.clicked.connect(self._pause_button_clicked)
         hbox.addWidget(self._pause_button)
 
         self._reset_button = QSliderButton("Reset")
         self._reset_button.clicked.connect(self._reset_button_clicked)
         hbox.addWidget(self._reset_button)
 
-
-
+        self.set_frames_per_second(PRESUMED_FRAMES_PER_SECOND)
 
     @property
     def frames_per_second(self):
-        return (1/PRESUMED_FRAMES_PER_SECOND)*1000
+        return self._frames_per_second
+
     @property
     def frame_duration(self):
-        return 1/self.frames_per_second
+        return self._frame_duration
+
+    def set_frames_per_second(self, frames_per_second):
+        self._frames_per_second = frames_per_second
+        self._frame_duration = 1.0 / frames_per_second
 
-    def set_slider_range(self,num_frames):
+    def set_slider_range(self, num_frames):
         self.slider_max = num_frames - 1
         self._slider.setValue(0)
         self._slider.setMaximum(self.slider_max)
 
     @pyqtSlot()
     def _timer_timeout(self):
         if self._slider.value() < self.slider_max:
             self._slider.setValue(self._slider.value() + 1)
         else:
             self._slider.setValue(0)
 
     @pyqtSlot()
     def _play_button_clicked(self):
         self._timer.stop()
-        # self._timer.start(int(self.frame_duration))
-        self._timer.start(0) #play as fast as possible
-
-    @pyqtSlot()
-    def _play_double_speed_button_clicked(self):
-        self._timer.stop()
-        self._timer.start(int(self.frame_duration/2))
-
-    @pyqtSlot()
-    def _play_half_speed_button_clicked(self):
-        self._timer.stop()
-        self._timer.start(int(self.frame_duration*2))
+        self._timer.start(0)  # play as fast as possible
 
     @pyqtSlot()
     def _pause_button_clicked(self):
         self._timer.stop()
 
     @pyqtSlot()
     def _reset_button_clicked(self):
         self._timer.stop()
-        self._slider.setValue(0)
+        self._slider.setValue(0)
```

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/marker_selector_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/sub_widgets/time_series_viewer_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py` & `skelly_viewer-2023.5.1018/skelly_viewer/gui/qt/widgets/time_series_widgets/trajectory_view_widget.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/utilities/freemocap_data_loader.py` & `skelly_viewer-2023.5.1018/skelly_viewer/utilities/freemocap_data_loader.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/utilities/load_sample_data.py` & `skelly_viewer-2023.5.1018/skelly_viewer/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/utilities/mediapipe_skeleton_builder.py` & `skelly_viewer-2023.5.1018/skelly_viewer/utilities/mediapipe_skeleton_builder.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/skelly_viewer/utilities/video_handler.py` & `skelly_viewer-2023.5.1018/skelly_viewer/utilities/video_handler.py`

 * *Files identical despite different names*

### Comparing `skelly_viewer-2023.3.1017/PKG-INFO` & `skelly_viewer-2023.5.1018/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skelly_viewer
-Version: 2023.3.1017
+Version: 2023.5.1018
 Summary: View a skelly
 Keywords: basic,template,python,repository
 Author-email: Skelly FreeMoCap <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
```

