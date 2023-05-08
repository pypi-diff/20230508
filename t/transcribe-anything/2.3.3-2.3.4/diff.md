# Comparing `tmp/transcribe-anything-2.3.3.tar.gz` & `tmp/transcribe-anything-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe-anything-2.3.3.tar", last modified: Sat May  6 00:04:52 2023, max compression
+gzip compressed data, was "transcribe-anything-2.3.4.tar", last modified: Mon May  8 10:09:37 2023, max compression
```

## Comparing `transcribe-anything-2.3.3.tar` & `transcribe-anything-2.3.4.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 00:04:52.396520 transcribe-anything-2.3.3/
--rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.3.3/LICENSE
--rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     9120 2023-05-06 00:04:52.396520 transcribe-anything-2.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     8096 2023-05-05 23:45:46.000000 transcribe-anything-2.3.3/README.md
--rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.3.3/requirements.testing.txt
--rw-rw-rw-   0        0        0       71 2023-05-05 22:22:57.000000 transcribe-anything-2.3.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 00:04:52.397520 transcribe-anything-2.3.3/setup.cfg
--rw-rw-rw-   0        0        0     3109 2023-05-05 23:46:31.000000 transcribe-anything-2.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 00:04:52.368519 transcribe-anything-2.3.3/tests/
--rw-rw-rw-   0        0        0     2794 2023-05-05 18:57:48.000000 transcribe-anything-2.3.3/tests/test_transcribe_anything.py
--rw-rw-rw-   0        0        0      449 2022-12-01 20:48:45.000000 transcribe-anything-2.3.3/tests/test_whisper.py
-drwxrwxrwx   0        0        0        0 2023-05-06 00:04:52.376521 transcribe-anything-2.3.3/transcribe_anything/
--rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.3.3/transcribe_anything/__init__.py
--rw-rw-rw-   0        0        0     5289 2023-05-05 23:50:24.000000 transcribe-anything-2.3.3/transcribe_anything/api.py
--rw-rw-rw-   0        0        0     3071 2023-03-20 23:48:49.000000 transcribe-anything-2.3.3/transcribe_anything/audio.py
--rw-rw-rw-   0        0        0     2836 2023-05-05 22:22:52.000000 transcribe-anything-2.3.3/transcribe_anything/cmd.py
--rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.3.3/transcribe_anything/logger.py
--rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.3.3/transcribe_anything/parse_whisper_options.py
--rw-rw-rw-   0        0        0     1536 2023-05-05 23:48:52.000000 transcribe-anything-2.3.3/transcribe_anything/util.py
-drwxrwxrwx   0        0        0        0 2023-05-06 00:04:52.395518 transcribe-anything-2.3.3/transcribe_anything.egg-info/
--rw-rw-rw-   0        0        0     9120 2023-05-06 00:04:52.000000 transcribe-anything-2.3.3/transcribe_anything.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      614 2023-05-06 00:04:52.000000 transcribe-anything-2.3.3/transcribe_anything.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 00:04:52.000000 transcribe-anything-2.3.3/transcribe_anything.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2023-05-06 00:04:52.000000 transcribe-anything-2.3.3/transcribe_anything.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       71 2023-05-06 00:04:52.000000 transcribe-anything-2.3.3/transcribe_anything.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-06 00:04:52.000000 transcribe-anything-2.3.3/transcribe_anything.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.277005 transcribe-anything-2.3.4/
+-rw-rw-rw-   0        0        0     1064 2022-12-01 20:48:45.000000 transcribe-anything-2.3.4/LICENSE
+-rw-rw-rw-   0        0        0       57 2022-12-01 20:48:45.000000 transcribe-anything-2.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     9256 2023-05-08 10:09:37.277005 transcribe-anything-2.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8231 2023-05-08 07:32:22.000000 transcribe-anything-2.3.4/README.md
+-rw-rw-rw-   0        0        0       24 2022-12-01 20:48:45.000000 transcribe-anything-2.3.4/requirements.testing.txt
+-rw-rw-rw-   0        0        0       71 2023-05-05 22:22:57.000000 transcribe-anything-2.3.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 10:09:37.278002 transcribe-anything-2.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     3109 2023-05-08 07:31:13.000000 transcribe-anything-2.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.243003 transcribe-anything-2.3.4/tests/
+-rw-rw-rw-   0        0        0      808 2023-05-08 09:56:56.000000 transcribe-anything-2.3.4/tests/test_local_file_cmd.py
+-rw-rw-rw-   0        0        0     2813 2023-05-08 09:15:57.000000 transcribe-anything-2.3.4/tests/test_transcribe_anything.py
+-rw-rw-rw-   0        0        0     2110 2023-05-08 09:47:26.000000 transcribe-anything-2.3.4/tests/test_transcribe_anything_api.py
+-rw-rw-rw-   0        0        0      449 2023-05-08 09:15:57.000000 transcribe-anything-2.3.4/tests/test_whisper.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.250008 transcribe-anything-2.3.4/transcribe_anything/
+-rw-rw-rw-   0        0        0        0 2022-12-08 07:42:26.000000 transcribe-anything-2.3.4/transcribe_anything/__init__.py
+-rw-rw-rw-   0        0        0     6003 2023-05-08 09:49:04.000000 transcribe-anything-2.3.4/transcribe_anything/api.py
+-rw-rw-rw-   0        0        0     3740 2023-05-08 09:06:47.000000 transcribe-anything-2.3.4/transcribe_anything/audio.py
+-rw-rw-rw-   0        0        0     2598 2023-05-08 07:34:00.000000 transcribe-anything-2.3.4/transcribe_anything/cmd.py
+-rw-rw-rw-   0        0        0      613 2022-12-03 03:51:42.000000 transcribe-anything-2.3.4/transcribe_anything/logger.py
+-rw-rw-rw-   0        0        0     1210 2022-12-03 03:51:42.000000 transcribe-anything-2.3.4/transcribe_anything/parse_whisper_options.py
+-rw-rw-rw-   0        0        0     1536 2023-05-05 23:48:52.000000 transcribe-anything-2.3.4/transcribe_anything/util.py
+drwxrwxrwx   0        0        0        0 2023-05-08 10:09:37.276004 transcribe-anything-2.3.4/transcribe_anything.egg-info/
+-rw-rw-rw-   0        0        0     9256 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      681 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-08 10:09:37.000000 transcribe-anything-2.3.4/transcribe_anything.egg-info/top_level.txt
```

### Comparing `transcribe-anything-2.3.3/LICENSE` & `transcribe-anything-2.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.3/PKG-INFO` & `transcribe-anything-2.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.3.3
+Version: 2.3.4
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -163,14 +163,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
   * 2.3.3: Fix case where there spaces in name (happens on windows)
   * 2.3.2: Fix windows transcoding error
   * 2.3.1: static-ffmpeg >= 2.5 now specified
   * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
```

### Comparing `transcribe-anything-2.3.3/README.md` & `transcribe-anything-2.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
   * 2.3.3: Fix case where there spaces in name (happens on windows)
   * 2.3.2: Fix windows transcoding error
   * 2.3.1: static-ffmpeg >= 2.5 now specified
   * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
```

### Comparing `transcribe-anything-2.3.3/setup.py` & `transcribe-anything-2.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "Uses whisper AI to transcribe speach from video and audio files. "
     "Also accepts urls for youtube, rumble, bitchute, clear file, etc."
 )
 URL = "https://github.com/zackees/transcribe-anything"
 EMAIL = "dont@email.me"
 AUTHOR = "Zach Vorhies"
 REQUIRES_PYTHON = ">=3.9.0"
-VERSION = "2.3.3"
+VERSION = "2.3.4"
 
 # The text of the README file
 with open(os.path.join(HERE, "README.md"), encoding="utf-8", mode="r") as fd:
     README = fd.read()
 
 
 def parse_requirements(filename):
```

### Comparing `transcribe-anything-2.3.3/tests/test_transcribe_anything.py` & `transcribe-anything-2.3.4/tests/test_transcribe_anything.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,20 +60,21 @@
             "transcribe_anything https://www.youtube.com/watch?v=DWtpNPZ4tb4"
             f" --model tiny --output_dir {TESTS_DATA_DIR}"
         )
         rtn_val = subprocess.call(cmd, shell=True)
         self.assertEqual(rtn_val, 0, "command failed")
         expected_paths = [
             TESTS_DATA_DIR,
-            os.path.join(TESTS_DATA_DIR, "out.mp3"),
+            # os.path.join(TESTS_DATA_DIR, "out.mp3"),
             os.path.join(TESTS_DATA_DIR, "out.txt"),
             os.path.join(TESTS_DATA_DIR, "out.srt"),
             os.path.join(TESTS_DATA_DIR, "out.vtt"),
         ]
         for expected_path in expected_paths:
             self.assertTrue(
-                os.path.exists(expected_path), f"expected path {expected_path} not found"
+                os.path.exists(expected_path),
+                f"expected path {expected_path} not found",
             )
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `transcribe-anything-2.3.3/transcribe_anything/api.py` & `transcribe-anything-2.3.4/transcribe_anything/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,62 @@
 """
     Api for using transcribe_anything from python. Allows bulk processing.
 """
 
 # pylint: disable=too-many-arguments,broad-except,too-many-locals,unsupported-binary-operation,too-many-branches,too-many-statements
 
+import atexit
 import os
 import stat
 import sys
 import time
 import subprocess
-import shutil
 from typing import Optional
+import tempfile
+import shutil
 
-from static_ffmpeg import add_paths  # type: ignore
+from static_ffmpeg import add_paths as ffmpeg_add_paths  # type: ignore
 
 from transcribe_anything.audio import fetch_audio
 from transcribe_anything.util import (
     get_computing_device,
     sanitize_filename,
     chop_double_extension,
 )
 from transcribe_anything.logger import log_error
 
 PERMS = stat.S_IRUSR | stat.S_IRGRP | stat.S_IROTH | stat.S_IWOTH | stat.S_IWUSR | stat.S_IWGRP
 
-add_paths()
+ffmpeg_add_paths()
+
+
+def make_temp_wav() -> str:
+    """
+    Makes a temporary mp3 file and returns the path to it.
+    """
+    tmp = tempfile.NamedTemporaryFile(  # pylint: disable=consider-using-with
+        suffix=".wav", delete=False
+    )
+
+    tmp.close()
+
+    def cleanup() -> None:
+        if os.path.exists(tmp.name):
+            os.remove(tmp.name)
+
+    atexit.register(cleanup)
+    return tmp.name
 
 
 def transcribe(
     url_or_file: str,
     output_dir: Optional[str] = None,
     model: Optional[str] = None,
     task: Optional[str] = None,
     language: Optional[str] = None,
-    keep_audio: bool = False,
     device: Optional[str] = None,
     other_args: Optional[list[str]] = None,
 ) -> str:
     """
     Runs the program.
     """
     basename = os.path.basename(url_or_file)
@@ -65,80 +84,82 @@
                 log_error("yt-dlp failed to get title, using basename instead.")
                 output_dir = "text_" + basename
         else:
             output_dir = "text_" + os.path.splitext(basename)[0]
     if output_dir_was_generated and language is not None:
         output_dir = os.path.join(output_dir, language)
     print(f"making dir {output_dir}")
-    if os.path.isdir(output_dir):
-        shutil.rmtree(output_dir, ignore_errors=True)
     os.makedirs(output_dir, exist_ok=True)
+    tmp_wav = make_temp_wav()
     assert os.path.isdir(output_dir), f"Path {output_dir} is not found or not a directory."
-    tmp_mp3 = os.path.join(output_dir, "out.mp3")
-    fetch_audio(url_or_file, tmp_mp3)
-    assert os.path.exists(tmp_mp3), f"Path {tmp_mp3} doesn't exist."
+    # tmp_mp3 = os.path.join(output_dir, "out.mp3")
+    fetch_audio(url_or_file, tmp_wav)
+    assert os.path.exists(tmp_wav), f"Path {tmp_wav} doesn't exist."
     device = device or get_computing_device()
     if device == "cuda":
         print("#####################################")
         print("######### GPU ACCELERATED! ##########")
         print("#####################################")
     elif device == "cpu":
         print("WARNING: NOT using GPU acceleration, using 10x slower CPU instead.")
     else:
         raise ValueError(f"Unknown device {device}")
     print(f"Using device {device}")
     model_str = f" --model {model}" if model else ""
-    output_dir_str = f' --output_dir "{output_dir}"' if output_dir else ""
     task_str = f" --task {task}" if task else ""
     language_str = f" --language {language}" if language else ""
     cmd_list = []
     if sys.platform == "win32":
+        # Set the text mode to UTF-8 on Windows.
         cmd_list.extend(["chcp", "65001", "&&"])
-    cmd_list.extend(
-        [
-            "whisper",
-            f'"{tmp_mp3}"',
-            "--device",
-            device,
-            model_str,
-            output_dir_str,
-            task_str,
-            language_str,
-        ]
-    )
-    if other_args:
-        cmd_list.extend(other_args)
-    # Remove the empty strings.
-    cmd_list = [x.strip() for x in cmd_list if x.strip()]
-    cmd = " ".join(cmd_list)
-    sys.stderr.write(f"Running:\n  {cmd}\n")
-    proc = subprocess.Popen(  # pylint: disable=consider-using-with
-        cmd, shell=True, universal_newlines=True
-    )
-    while True:
-        rtn = proc.poll()
-        if rtn is None:
-            time.sleep(0.25)
-            continue
-        if rtn != 0:
-            msg = f"Failed to execute {cmd}\n "
-            raise OSError(msg)
-        break
-    files = [os.path.join(output_dir, name) for name in os.listdir(output_dir)]
-    for file in files:
-        # Change the filename to remove the double extension
-        file_name = os.path.basename(file)
-        base_path = os.path.dirname(file)
-        new_file = os.path.join(base_path, chop_double_extension(file_name))
-        if file != new_file:
-            if os.path.exists(new_file):
-                os.remove(new_file)
-            os.rename(file, new_file)
-    if not keep_audio:
-        os.remove(tmp_mp3)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        cmd_list.extend(
+            [
+                "whisper",
+                f'"{tmp_wav}"',
+                "--device",
+                device,
+                model_str,
+                f'--output_dir "{tmpdir}"',
+                task_str,
+                language_str,
+            ]
+        )
+        if other_args:
+            cmd_list.extend(other_args)
+        # Remove the empty strings.
+        cmd_list = [x.strip() for x in cmd_list if x.strip()]
+        cmd = " ".join(cmd_list)
+        sys.stderr.write(f"Running:\n  {cmd}\n")
+        proc = subprocess.Popen(  # pylint: disable=consider-using-with
+            cmd, shell=True, universal_newlines=True
+        )
+        while True:
+            rtn = proc.poll()
+            if rtn is None:
+                time.sleep(0.25)
+                continue
+            if rtn != 0:
+                msg = f"Failed to execute {cmd}\n "
+                raise OSError(msg)
+            break
+        files = [os.path.join(tmpdir, name) for name in os.listdir(tmpdir)]
+        for file in files:
+            # Change the filename to remove the double extension
+            file_name = os.path.basename(file)
+            base_path = os.path.dirname(file)
+            new_file = os.path.join(base_path, chop_double_extension(file_name))
+            _, ext = os.path.splitext(new_file)
+            outfile = os.path.join(output_dir, f"out{ext}")
+            if os.path.exists(outfile):
+                os.remove(outfile)
+            assert os.path.isfile(file), f"Path {file} doesn't exist."
+            assert not os.path.exists(outfile), f"Path {outfile} already exists."
+            shutil.move(file, outfile)
     return output_dir
 
 
 if __name__ == "__main__":
     # test case for twitter video
     # transcribe(url_or_file="https://twitter.com/wlctv_ca/status/1598895698870951943")
     try:
```

### Comparing `transcribe-anything-2.3.3/transcribe_anything/audio.py` & `transcribe-anything-2.3.4/transcribe_anything/audio.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 
 import sys
 import tempfile
 import subprocess
 import os
+import shutil
 import static_ffmpeg  # type: ignore
 
 _PROCESS_TIMEOUT = 4 * 60 * 60
 
 
 def _ytdlp_download(url: str, outdir: str) -> str:
     """Downloads a file using ytdlp."""
@@ -31,52 +32,71 @@
     new_files = os.listdir(outdir)
     assert len(new_files) == 1, f"Expected 1 file, got {new_files}"
     downloaded_file = os.path.join(outdir, new_files[0])
     assert os.path.exists(downloaded_file), f"The expected file {downloaded_file} doesn't exist"
     return downloaded_file
 
 
-def _convert_to_mp3(inpath: str, outpath: str, speech_normalization: bool = False) -> None:
-    """Converts a file to mp3."""
+def _convert_to_wav(inpath: str, outpath: str, speech_normalization: bool = False) -> None:
+    """Converts a file to wav."""
     cmd_audio_filter = ""
     if speech_normalization:
         cmd_audio_filter = "-filter:a speechnorm=e=12.5:r=0.00001:l=1"
-    cmd = f'ffmpeg -y -i "{inpath}" {cmd_audio_filter} -acodec libmp3lame "{outpath}"'
+    tmpwav = tempfile.NamedTemporaryFile(  # pylint: disable=consider-using-with
+        suffix=".wav", delete=False
+    )
+    tmpwav.close()
+    tmpwavepath = tmpwav.name
+    audio_encoder = "-acodec pcm_s16le -ar 44100 -ac 1"
+    cmd = f'ffmpeg -y -i "{inpath}" {cmd_audio_filter} {audio_encoder} "{tmpwavepath}"'
     print(f"Running:\n  {cmd}")
     try:
         subprocess.run(cmd, shell=True, check=True, capture_output=True, timeout=_PROCESS_TIMEOUT)
     except subprocess.CalledProcessError as exc:
         print(f"Failed to run {cmd} with error {exc}")
         print(f"stdout: {exc.stdout}")
         print(f"stderr: {exc.stderr}")
         raise
+    os.remove(outpath)
+    os.rename(tmpwavepath, outpath)
     assert os.path.exists(outpath), f"The expected file {outpath} doesn't exist"
 
 
-def fetch_audio(url_or_file: str, out_mp3: str) -> None:
+def fetch_audio(url_or_file: str, out_wav: str) -> None:
     """Fetches from the internet or from a local file and outputs a wav file."""
-    assert out_mp3.endswith(".mp3")
+    assert out_wav.endswith(".wav")
     static_ffmpeg.add_paths()  # pylint: disable=no-member
     if url_or_file.startswith("http") or url_or_file.startswith("ftp"):
         with tempfile.TemporaryDirectory() as tmpdir:
             print(f"Using temporary directory {tmpdir}")
             downloaded_file = _ytdlp_download(url_or_file, os.path.abspath(tmpdir))
             print("Downloaded file: ", downloaded_file)
-            _convert_to_mp3(downloaded_file, out_mp3, speech_normalization=True)
+            _convert_to_wav(downloaded_file, out_wav, speech_normalization=True)
         sys.stderr.write("Downloading complete.\n")
-        assert os.path.exists(out_mp3), f"The expected file {out_mp3} doesn't exist"
+        assert os.path.exists(out_wav), f"The expected file {out_wav} doesn't exist"
     else:
         assert os.path.isfile(url_or_file)
-        cmd = f'ffmpeg -i "{url_or_file}" -acodec libmp3lame "{out_mp3}"'
-        sys.stderr.write(f"Running:\n  {cmd}\n")
-        subprocess.run(cmd, shell=True, check=True, capture_output=True, timeout=_PROCESS_TIMEOUT)
-        assert os.path.exists(out_mp3), f"The expected file {out_mp3} doesn't exist"
+        abspath = os.path.abspath(url_or_file)
+        out_wav_abs = os.path.abspath(out_wav)
+        with tempfile.TemporaryDirectory() as tmpdir:
+            cmd = f'ffmpeg -y -i "{abspath}" -acodec pcm_s16le -ar 44100 -ac 1 out.wav'
+            sys.stderr.write(f"Running:\n  {cmd}\n")
+            subprocess.run(
+                cmd,
+                cwd=tmpdir,
+                shell=True,
+                check=True,
+                capture_output=True,
+                timeout=_PROCESS_TIMEOUT,
+            )
+            shutil.copyfile(os.path.join(tmpdir, "out.wav"), out_wav_abs)
+        assert os.path.exists(out_wav), f"The expected file {out_wav} doesn't exist"
 
 
 def unit_test() -> None:
     """Runs the program."""
     url = "https://www.youtube.com/watch?v=8Wg8f2g_GQY"
-    fetch_audio(url, "out.mp3")
+    fetch_audio(url, "out.wav")
 
 
 if __name__ == "__main__":
     unit_test()
```

### Comparing `transcribe-anything-2.3.3/transcribe_anything/cmd.py` & `transcribe-anything-2.3.4/transcribe_anything/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,21 +43,14 @@
     )
     parser.add_argument(
         "--language",
         help="language to the target audio is in, default None will auto-detect",
         default=None,
         choices=[None] + whisper_options["language"],
     )
-    # keep_audio
-    parser.add_argument(
-        "--no-keep-audio",
-        help="whether to keep the audio file after processing",
-        default=False,
-        action="store_true",
-    )
     parser.add_argument(
         "--device",
         help="device to use for processing, None will auto select CUDA if available or else CPU",
         default=None,
         choices=[None, "cpu", "cuda"],
     )
     # add extra options that are passed into the transcribe function
@@ -67,22 +60,21 @@
     try:
         transcribe(
             url_or_file=args.url_or_file,
             output_dir=args.output_dir,
             model=args.model if args.model != "None" else None,
             task=args.task,
             language=args.language if args.language != "None" else None,
-            keep_audio=not args.no_keep_audio,
             device=args.device,
             other_args=unknown,
         )
     except KeyboardInterrupt:
         print("KeyboardInterrupt")
         return 1
     return 0
 
 
 if __name__ == "__main__":
     # push sys argv prior to call
-    sys.argv.append("test.mp3")
+    sys.argv.append("test.wav")
     sys.argv.append('--initial_prompt "What is your name?"')
     sys.exit(main())
```

### Comparing `transcribe-anything-2.3.3/transcribe_anything/logger.py` & `transcribe-anything-2.3.4/transcribe_anything/logger.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.3/transcribe_anything/parse_whisper_options.py` & `transcribe-anything-2.3.4/transcribe_anything/parse_whisper_options.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.3/transcribe_anything/util.py` & `transcribe-anything-2.3.4/transcribe_anything/util.py`

 * *Files identical despite different names*

### Comparing `transcribe-anything-2.3.3/transcribe_anything.egg-info/PKG-INFO` & `transcribe-anything-2.3.4/transcribe_anything.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-anything
-Version: 2.3.3
+Version: 2.3.4
 Summary: Uses whisper AI to transcribe speach from video and audio files. Also accepts urls for youtube, rumble, bitchute, clear file, etc.
 Home-page: https://github.com/zackees/transcribe-anything
 Author: Zach Vorhies
 Author-email: dont@email.me
 License: MIT
 Keywords: transcription translation speech-to-text speech-recognition command-line-tool ai whisper ml anything
 Classifier: License :: OSI Approved :: MIT License
@@ -163,14 +163,15 @@
     * github: https://github.com/zackees/static_ffmpeg
     * pypi: https://pypi.org/project/static-ffmpeg/
 
 # Testing
   * All tests are run by `tox`, simply go to the project directory root and run it.
 
 # Versions
+  * 2.3.4: Removed `out.mp3` and instead use a temporary wav file, as that is faster to process. --no-keep-audio has now been removed.
   * 2.3.3: Fix case where there spaces in name (happens on windows)
   * 2.3.2: Fix windows transcoding error
   * 2.3.1: static-ffmpeg >= 2.5 now specified
   * 2.3.0: Now uses the official version of whisper ai
   * 2.2.1: "test_" is now prepended to all the different output folder names.
   * 2.2.0: Now explictly setting a language will put the file in a folder with that language name, allowing multi language passes without overwriting.
   * 2.1.2: yt-dlp pinned to new minimum version. Fixes downloading issues from old lib. Adds audio normalization by default.
```

### Comparing `transcribe-anything-2.3.3/transcribe_anything.egg-info/SOURCES.txt` & `transcribe-anything-2.3.4/transcribe_anything.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.testing.txt
 requirements.txt
 setup.py
+tests/test_local_file_cmd.py
 tests/test_transcribe_anything.py
+tests/test_transcribe_anything_api.py
 tests/test_whisper.py
 transcribe_anything/__init__.py
 transcribe_anything/api.py
 transcribe_anything/audio.py
 transcribe_anything/cmd.py
 transcribe_anything/logger.py
 transcribe_anything/parse_whisper_options.py
```

