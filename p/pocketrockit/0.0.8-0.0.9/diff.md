# Comparing `tmp/pocketrockit-0.0.8.tar.gz` & `tmp/pocketrockit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pocketrockit-0.0.8.tar", max compression
+gzip compressed data, was "pocketrockit-0.0.9.tar", max compression
```

## Comparing `pocketrockit-0.0.8.tar` & `pocketrockit-0.0.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2639 2023-04-25 05:45:46.696906 pocketrockit-0.0.8/Readme.md
--rw-r--r--   0        0        0        0 2023-04-25 05:45:46.700907 pocketrockit-0.0.8/pocketrockit/__init__.py
--rwxr-xr-x   0        0        0     1015 2023-04-25 05:45:46.700907 pocketrockit-0.0.8/pocketrockit/cli.py
--rwxr-xr-x   0        0        0    12410 2023-04-25 08:48:14.457679 pocketrockit-0.0.8/pocketrockit/decorated.py
--rwxr-xr-x   0        0        0     9522 2023-04-25 09:05:44.584263 pocketrockit-0.0.8/pocketrockit/engine.py
--rw-r--r--   0        0        0     1890 2023-04-25 09:06:04.932314 pocketrockit-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pocketrockit-0.0.8/setup.py
--rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pocketrockit-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2639 2023-04-25 05:45:46.696906 pocketrockit-0.0.9/Readme.md
+-rw-r--r--   0        0        0      136 2023-04-25 09:35:28.121306 pocketrockit-0.0.9/pocketrockit/__init__.py
+-rwxr-xr-x   0        0        0     1015 2023-04-25 05:45:46.700907 pocketrockit-0.0.9/pocketrockit/cli.py
+-rwxr-xr-x   0        0        0    12449 2023-04-25 12:35:43.398410 pocketrockit-0.0.9/pocketrockit/decorated.py
+-rwxr-xr-x   0        0        0     9760 2023-04-25 12:50:35.256352 pocketrockit-0.0.9/pocketrockit/engine.py
+-rw-r--r--   0        0        0     1890 2023-04-25 13:40:07.215499 pocketrockit-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pocketrockit-0.0.9/setup.py
+-rw-r--r--   0        0        0     3228 1970-01-01 00:00:00.000000 pocketrockit-0.0.9/PKG-INFO
```

### Comparing `pocketrockit-0.0.8/Readme.md` & `pocketrockit-0.0.9/Readme.md`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.8/pocketrockit/cli.py` & `pocketrockit-0.0.9/pocketrockit/cli.py`

 * *Files identical despite different names*

### Comparing `pocketrockit-0.0.8/pocketrockit/decorated.py` & `pocketrockit-0.0.9/pocketrockit/decorated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 """API for fancy decorator based track definitions"""
 
 from collections.abc import Sequence
-from itertools import count
 from functools import wraps
+from itertools import count
 
 from pocketrockit.engine import Env, Stage, run
 
 stage = Stage()
 
 __all__ = ["track", "player", "Env", "midiseq"]
 
@@ -107,45 +107,47 @@
     if note_str[0] in {"t", "n"}:
         return scale[int(note_str[1]) - 1] + shift
     return NOTES[note_str] + shift
 
 
 def midi_commands(string: str, channel: int, force_note: None | str, scale, velocity: int):
     """Turns something like '60', 'c', 'c,d,e' or 't1,t2,t3' into MIDI commands"""
-
     try:
         return (
             []
             if string == "."
             else [
                 (
                     channel,
-                    force_note if isinstance(force_note, int) else resolve(force_note or element, scale),
+                    force_note
+                    if isinstance(force_note, int)
+                    else resolve(force_note or element, scale),
                     velocity,
                 )
                 for element in string.split(",")
             ]
         )
     except Exception as exc:  # pylint: disable=broad-except
         print(f"could not turn '{string}' into note ({exc})")
         return []
 
 
 def midi_terminator(midi_fn):
     """Cleans up"""
     active = {}
+
     @wraps(midi_fn)
     def cleanup(*args, **kwargs):
-        gen =  midi_fn(*args, **kwargs)
+        gen = midi_fn(*args, **kwargs)
         comm = None
         for i in count():
             stoppers = []
             loop, tick, original, commands = gen.send(comm)
             for channel, note, _velocity in commands or []:
-                #print((channel, note), active)
+                # print((channel, note), active)
                 if (channel, note) in active:
                     stoppers.append((channel, note, None))
                     del active[channel, note]
 
                 for (c, n), store_tick in list(active.items()):
                     if i - store_tick > 0:
                         stoppers.append((c, n, None))
@@ -304,15 +306,14 @@
         (126, {"fis’’’’’’", "126", "ges’’’’’’", "Gb9", "F#9"}, 11839.82),
         (127, {"G9", "g’’’’’’", "127"}, 12543.85),
     )
     for name in names
 }
 
 
-
 if __name__ == "__main__":
     note_generator = midiseq("x " * 16)
     print(note_generator.send(None))
     print(note_generator.send(None))
 
     print(note_generator.send(1))
```

### Comparing `pocketrockit-0.0.8/pocketrockit/engine.py` & `pocketrockit-0.0.9/pocketrockit/engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 https://newt.phys.unsw.edu.au/jw/notes.html
 
 """
 
 import asyncio
 import logging
 import threading
-from asyncio import sleep
+import time
+from asyncio import sleep as async_sleep
 from collections.abc import Iterable, MutableMapping
 from contextlib import ExitStack, contextmanager, suppress
 from dataclasses import dataclass, field
 from importlib.util import module_from_spec, spec_from_file_location
 from itertools import count
 from pathlib import Path
 from types import ModuleType
@@ -185,15 +186,15 @@
 
 def terminate(terminator) -> None:
     terminator.set()
     pygame.event.post(pygame.event.Event(pygame.MOUSEMOTION))
 
 
 def logger() -> logging.Logger:
-    return logging.getLogger("silmaril")
+    return logging.getLogger("pocketrockit")
 
 
 def setup_logging() -> None:
     def thread_id_filter(record):
         """Inject thread_id to log records"""
         record.thread_id = threading.get_native_id()
         return record
@@ -204,35 +205,38 @@
     )
     handler.addFilter(thread_id_filter)
     logger().addHandler(handler)
     logger().setLevel("DEBUG")
 
 
 def load_module(filepath: str | Path) -> ModuleType:
+    """(Re)loads a python module specified by @filepath"""
     print(f"load module '{Path(filepath).stem}'")
     spec = spec_from_file_location(Path(filepath).stem, filepath)
     assert spec and spec.loader
     module = module_from_spec(spec)
     assert module
     # here the actual track definition takes place
     spec.loader.exec_module(module)
     return module
 
 
 async def music_loop() -> None:
+    """Main loop collecting instructions to send it to MIDI"""
     with mididevice_fluidsynth() as midi_out:
         # wait for players to emerge (otherwise `tick` won't start at 0)
         while True:
             if Stage().players:
                 break
             print("no players yet..")
-            await sleep(1)
+            await async_sleep(1)
             continue
 
         for tick in count():
+            last_now = time.time()
             Stage().tick = tick
 
             notes = []
             if tick % 1 == 0:
                 print(f"== {tick // 16} {tick // 4} {tick % 4} {tick} ==")
 
             for name, stream in Stage().players:
@@ -244,25 +248,24 @@
                 except StopIteration:
                     pass
                 except Exception as exc:  # pylint: disable=broad-except
                     print(f"exception in play: {exc}")
                     print("--")
 
             for channel, note, velocity in notes:
-
                 if velocity is None:
-                    #print("OF", (channel, note))
+                    # print("OF", (channel, note))
                     midi_out.noteoff(channel, note)
                 else:
-                    #print("ON", (channel, note, velocity))
+                    # print("ON", (channel, note, velocity))
                     midi_out.noteon(channel, note, velocity)
 
             # make me absolute please
             waitfor = 60 / Stage().env.bpm / 4
-            await sleep(waitfor)
+            await async_sleep(max(0, (waitfor - (time.time() - last_now))))
 
 
 async def watch_changes() -> None:
     """Watches for file changes in track definition file and reload on change"""
     stage = Stage()
     load_module(stage.file_to_track)
     with Inotify() as inotify:
```

### Comparing `pocketrockit-0.0.8/pyproject.toml` & `pocketrockit-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pocketrockit"
-version = "0.0.8"
+version = "0.0.9"
 description = "pocketrockit"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/pocketrockit.git"
 readme = "Readme.md"
 packages = [
   {include = "pocketrockit"}
 ]
```

### Comparing `pocketrockit-0.0.8/setup.py` & `pocketrockit-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 entry_points = \
 {'console_scripts': ['pocketrockit = pocketrockit.cli:main',
                      'pri = pocketrockit.cli:main']}
 
 setup_kwargs = {
     'name': 'pocketrockit',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'pocketrockit',
     'long_description': '# POCKETROCKIT - A rocket in your pocket that rocks!\n\n[Project page](https://projects.om-office.de/frans/pocketrockit.git)\n\nWrite a music track and play it while you write it. As you might know it from Sonic Pi, but in\nPython (`sonic.py` was not available on PyPi, though).\n\n\n## Usage\n\nWorkflow is not quite mature yet, so here is the short version for now.\n\nCreate and enter a development folder and provide required SoundFont files (configurable later,\nhard-coded for now)\n\n```sh\nmkdir mytracks\ncd mytracks\ncp /usr/share/soundfonts/FluidR3_GM.sf2 .\n```\n\nDownload [Roland JV-1080 Drums](https://musical-artifacts.com/artifacts/2744) (`JV_1080_Drums.sf2`)\nto that directory.\n\nCreate a file `myfirsttrack.py` with the following content:\n\n```python\n#!/usr/bin/env python3\n\nfrom pocketrockit.decorated import Env, midiseq, player, track\n\n@track\ndef po20(env: Env):\n    """A Pocket Operator PO-20 Arcade (well, not yet)"""\n\n    env.bpm = 60\n    key = "C3"\n\n    @player\n    def melody():\n        yield from midiseq(\n            " t6  t5  t6  t3 "\n            " t1  t3  t0  .  "\n            " .   .   .   .  "\n            " .   .   .   .  ",\n            key=key,\n            channel=25,\n        )\n\n    @player\n    def drums1():\n        yield from midiseq(\n            "x .  x  . "\n            "x .  .  . "\n            "x .  x  . "\n            "x .  x  x ",\n            channel=128,\n            note=33,\n        )\n```\n\nNow - keeping the editor open for later use - execute this file. You can either make it executable\nand run it directly or you run `python3` instead:\n\n```sh\nchmod +x myfirsttrack.py\n./myfirsttrack.py\n\n# or\n\npython3 myfirsttrack.py\n```\n\n\n## Installation\n\n```sh\n[<PYTHON> -m] pip[3] install [-U] pocketrockit\n```\n\n\n## Development & Contribution\n\n```sh\npip3 install -U poetry pre-commit\ngit clone --recurse-submodules https://projects.om-office.de/frans/pocketrockit.git\ncd pocketrockit\npre-commit install\n# if you need a specific version of Python inside your dev environment\npoetry env use ~/.pyenv/versions/3.10.4/bin/python3\npoetry install\n```\n\n\n## Stuff to read / Sources\n\n### SoundFonts\n\n* https://musescore.org/en/handbook/3/soundfonts-and-sfz-files\n* https://www.producersbuzz.com/category/downloads/download-free-soundfonts-sf2/\n* https://archive.org/details/500-soundfonts-full-gm-sets\n* https://ia802502.us.archive.org/view_archive.php?archive=/27/items/500-soundfonts-full-gm-sets/500_Soundfonts_Full_GM_Sets.zip\n* https://musical-artifacts.com/artifacts?formats=sf2&tags=soundfont\n\n\n### Music theory\n\n* https://pianoscales.org/major.html\n* https://www.inspiredacoustics.com/en/MIDI_note_numbers_and_center_frequencies\n',
     'author': 'Frans Fürst',
     'author_email': 'frans.fuerst+gitlab@protonmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://projects.om-office.de/frans/pocketrockit.git',
```

### Comparing `pocketrockit-0.0.8/PKG-INFO` & `pocketrockit-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pocketrockit
-Version: 0.0.8
+Version: 0.0.9
 Summary: pocketrockit
 Home-page: https://projects.om-office.de/frans/pocketrockit.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

