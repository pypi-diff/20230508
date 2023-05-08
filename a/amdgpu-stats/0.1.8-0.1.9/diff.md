# Comparing `tmp/amdgpu_stats-0.1.8.tar.gz` & `tmp/amdgpu_stats-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amdgpu_stats-0.1.8.tar", max compression
+gzip compressed data, was "amdgpu_stats-0.1.9.tar", max compression
```

## Comparing `amdgpu_stats-0.1.8.tar` & `amdgpu_stats-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.8/LICENSE.md
--rw-r--r--   0        0        0     2072 2023-04-26 03:40:20.512474 amdgpu_stats-0.1.8/README.md
--rw-r--r--   0        0        0      574 2023-04-26 05:05:44.845270 amdgpu_stats-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.8/src/amdgpu_stats/__init__.py
--rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.8/src/amdgpu_stats/amdgpu_stats.css
--rwxr-xr-x   0        0        0      343 2023-04-25 03:15:22.090179 amdgpu_stats-0.1.8/src/amdgpu_stats/amdgpu_stats.py
--rw-r--r--   0        0        0    10756 2023-04-25 06:31:39.246196 amdgpu_stats-0.1.8/src/amdgpu_stats/interface.py
--rw-r--r--   0        0        0     8885 2023-04-26 04:48:24.528350 amdgpu_stats-0.1.8/src/amdgpu_stats/utils.py
--rw-r--r--   0        0        0     3040 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.8/setup.py
--rw-r--r--   0        0        0     2845 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-04-23 18:43:59.684481 amdgpu_stats-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     2012 2023-04-27 04:34:37.246183 amdgpu_stats-0.1.9/README.md
+-rw-r--r--   0        0        0      574 2023-04-27 04:34:37.248183 amdgpu_stats-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-23 21:03:33.649030 amdgpu_stats-0.1.9/src/amdgpu_stats/__init__.py
+-rw-r--r--   0        0        0      393 2023-04-23 21:06:47.224510 amdgpu_stats-0.1.9/src/amdgpu_stats/amdgpu_stats.css
+-rwxr-xr-x   0        0        0      343 2023-04-25 03:15:22.090179 amdgpu_stats-0.1.9/src/amdgpu_stats/amdgpu_stats.py
+-rw-r--r--   0        0        0    11727 2023-04-27 04:34:37.248183 amdgpu_stats-0.1.9/src/amdgpu_stats/interface.py
+-rw-r--r--   0        0        0    10869 2023-04-27 04:34:37.248183 amdgpu_stats-0.1.9/src/amdgpu_stats/utils.py
+-rw-r--r--   0        0        0     2971 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.9/setup.py
+-rw-r--r--   0        0        0     2785 1970-01-01 00:00:00.000000 amdgpu_stats-0.1.9/PKG-INFO
```

### Comparing `amdgpu_stats-0.1.8/LICENSE.md` & `amdgpu_stats-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `amdgpu_stats-0.1.8/README.md` & `amdgpu_stats-0.1.9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 # amdgpu_stats
 
 A simple Python module/TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics
 
 ![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")
 
-![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")
-
 The GPU and temperature nodes (`edge`/`junction`/etc.) are discovered automatically.
 
-Statistics are not logged; only toggling Dark/light mode and the stat names / source files.
+Please see [the module section](#module) or [the docs](https://amdgpu-stats.readthedocs.io/en/latest/) for information on usage as an `import` in other tooling
 
 Tested _only_ on `RX6000` series cards; APUs and more _may_ be supported. Please file an issue if finding incompatibility!
 
 ## Requirements
 Only `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.
 
 It _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.
@@ -31,25 +29,24 @@
 
 *Rudimentary* support as a module exists; functions / variables offered can be found in `amdgpu_stats.utils`
 
 Demonstration:
 ```
 In [1]: import amdgpu_stats.utils
 
-In [2]: print(amdgpu_stats.utils.get_core_stats())
-{'sclk': 0, 'mclk': 1000000000, 'voltage': 0.01, 'util_pct': 0}
-
-In [3]: print(amdgpu_stats.utils.get_power_stats())
-{'limit': 281, 'average': 35, 'capability': 323, 'default': 281}
+In [2]: amdgpu_stats.utils.AMDGPU_CARDS
+Out[2]: {'card0': '/sys/class/drm/card0/device/hwmon/hwmon9'}
 
-In [4]: print(amdgpu_stats.utils.get_temp_stats())
-{'edge': 33, 'junction': 36, 'mem': 42}
+In [3]: amdgpu_stats.utils.get_core_stats('card0')
+Out[3]: {'sclk': 640000000, 'mclk': 1000000000, 'voltage': 0.79, 'util_pct': 65}
 
-In [5]: print(amdgpu_stats.utils.get_fan_stats())
-{'fan_rpm': 0, 'fan_rpm_target': 0}
+In [4]: amdgpu_stats.utils.get_clock('card0', 'core', format_freq=True)
+Out[4]: '659 MHz' 
 ```
+Feature requests [are encouraged](https://github.com/joshlay/amdgpu_stats/issues) :)
+
 ## Documentation
 
 For more information on the module, see:
  - `help('amdgpu_stats.utils')` in your interpreter
  - [ReadTheDocs](https://amdgpu-stats.readthedocs.io/en/latest/)
  - [the module source](https://github.com/joshlay/amdgpu_stats/blob/master/src/amdgpu_stats/utils.py) for more info
```

### Comparing `amdgpu_stats-0.1.8/pyproject.toml` & `amdgpu_stats-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "amdgpu-stats"
-version = "0.1.8"
+version = "0.1.9"
 description = "A simple module/TUI (using Textual) that provides AMD GPU statistics"
 authors = ["Josh Lay <pypi@jlay.io>"]
 repository = "https://github.com/joshlay/amdgpu_stats"
 license = "MIT"
 readme = "README.md"
 documentation = "https://amdgpu-stats.readthedocs.io/en/latest/"
```

### Comparing `amdgpu_stats-0.1.8/src/amdgpu_stats/interface.py` & `amdgpu_stats-0.1.9/src/amdgpu_stats/interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 from textual.binding import Binding
 from textual.app import App, ComposeResult
 from textual.containers import Container, Horizontal
 from textual.reactive import reactive
 from textual.screen import Screen
 from textual.widgets import Header, Footer, Static, TextLog, Label
 
-from .utils import CARD, SRC_FILES, TEMP_FILES, format_frequency, get_core_stats, get_fan_stats, get_power_stats, get_temp_stats  # pylint: disable=line-too-long
+from .utils import AMDGPU_CARDS, format_frequency, get_core_stats, get_fan_rpm, get_fan_target, get_power_stats, get_temp_stats  # pylint: disable=line-too-long
+
+# globals - card handling / choice for TUI
+if len(AMDGPU_CARDS) > 0:
+    # default to showing stats for the first detected card
+    CARD = next(iter(AMDGPU_CARDS))
+    hwmon_dir = AMDGPU_CARDS[CARD]
 
 
 class LogScreen(Screen):
     """Creates a screen for the logging widget"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -75,25 +81,26 @@
     ]
 
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
         yield Header()
         yield Container(GPUStatsWidget())
         self.update_log("[bold green]App started, logging begin!")
-        self.update_log("[bold italic]Information sources:[/]")
-        for metric, source in SRC_FILES.items():
-            self.update_log(f'[bold]  {metric}:[/] {source}')
-        for metric, source in TEMP_FILES.items():
-            self.update_log(f'[bold]  {metric} temperature:[/] {source}')
+        self.update_log(f"[bold italic]Information source:[/] {hwmon_dir}")
+        # nice-to-have: account for not storing these in dicts, but resolved in funcs
+        # for metric, source in SRC_FILES.items():
+        #    self.update_log(f'[bold]  {metric}:[/] {source}')
+        # for metric, source in TEMP_FILES.items():
+        #    self.update_log(f'[bold]  {metric} temperature:[/] {source}')
         yield Footer()
 
     def action_toggle_dark(self) -> None:
         """An action to toggle dark mode."""
         self.dark = not self.dark
-        self.update_log(f"Dark side: [bold]{self.dark}")
+        self.update_log(f"[bold]Dark side: [italic]{self.dark}")
 
     def action_quit_app(self) -> None:
         """An action to quit the program"""
         message = "Exiting on user request"
         self.update_log(f"[bold]{message}")
         self.exit(message)
 
@@ -110,63 +117,82 @@
         log_screen.text_log.write(message)
 
 
 class MiscDisplay(Static):
     """A widget to display misc. GPU stats."""
     # construct the misc. stats dict; appended by discovered temperature nodes
     # used to make a 'reactive' object
-    fan_stats = reactive({"fan_rpm": 0,
-                          "fan_rpm_target": 0})
+    fan_rpm = reactive(0)
+    fan_rpm_target = reactive(0)
+    # do some dancing to craft the UI; initialize the reactive obj with data
+    # to get proper labels
+    initial_stats = get_temp_stats(CARD)
+    # dynamic object for temperature updates
     temp_stats = reactive({})
+    # default to 'not composed', once labels are made - become true
+    # avoids a race condition between discovering temperature nodes/stats
+    # ... and making labels for them
+    composed = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.timer_misc = None
+        self.temp_stats = get_temp_stats(CARD)
 
     def compose(self) -> ComposeResult:
         yield Horizontal(Label("[underline]Temperatures"),
                          Label("", classes="statvalue"))
-        for temp_node in TEMP_FILES:
+        for temp_node in self.initial_stats:
             # capitalize the first letter for display
             caption = temp_node[0].upper() + temp_node[1:]
             yield Horizontal(Label(f'  {caption}:',),
-                             Label("", id="temp_" + temp_node, classes="statvalue"))
+                             Label("", id="temp_" + temp_node,
+                                   classes="statvalue"))
         yield Horizontal(Label("[underline]Fan RPM"),
                          Label("", classes="statvalue"))
         yield Horizontal(Label("  Current:",),
                          Label("", id="fan_rpm", classes="statvalue"))
         yield Horizontal(Label("  Target:",),
                          Label("", id="fan_rpm_target", classes="statvalue"))
+        self.composed = True
 
     def on_mount(self) -> None:
         """Event handler called when widget is added to the app."""
         self.timer_misc = self.set_interval(1, self.update_misc_stats)
 
     def update_misc_stats(self) -> None:
         """Method to update the temp/fan values to current measurements.
 
         Run by a timer created 'on_mount'"""
-        self.fan_stats = get_fan_stats()
-        self.temp_stats = get_temp_stats()
+        self.fan_rpm = get_fan_rpm(CARD)
+        self.fan_rpm_target = get_fan_target(CARD)
+        self.temp_stats = get_temp_stats(CARD)
+
+    def watch_fan_rpm(self, fan_rpm: int) -> None:
+        """Called when the 'fan_rpm' reactive attr changes.
+
+         - Updates label values
+         - Casting inputs to string to avoid type problems w/ int/None"""
+        self.query_one("#fan_rpm", Static).update(f"{fan_rpm}")
 
-    def watch_fan_stats(self, fan_stats: dict) -> None:
-        """Called when the 'fan_stats' reactive attr changes.
+    def watch_fan_rpm_target(self, fan_rpm_target: int) -> None:
+        """Called when the 'fan_rpm_target' reactive attr changes.
 
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
-        self.query_one("#fan_rpm", Static).update(f"{fan_stats['fan_rpm']}")
-        self.query_one("#fan_rpm_target", Static).update(f"{fan_stats['fan_rpm_target']}")
+        self.query_one("#fan_rpm_target", Static).update(f"{fan_rpm_target}")
 
     def watch_temp_stats(self, temp_stats: dict) -> None:
         """Called when the temp_stats reactive attr changes, updates labels"""
-        for temp_node in TEMP_FILES:
-            # check first if the reactive object has been updated with keys
-            if temp_node in temp_stats:
-                stat_dict_item = temp_stats[temp_node]
-                self.query_one("#temp_" + temp_node, Static).update(f'{stat_dict_item}C')
+        # try to avoid racing
+        if not self.composed:
+            return
+        for temp_node in temp_stats:
+            item_val = self.temp_stats[temp_node]
+            self.query_one("#temp_" + temp_node, Static).update(f'{item_val}C')
 
 
 class ClockDisplay(Static):
     """A widget to display GPU power stats."""
     core_vals = reactive({"sclk": 0, "mclk": 0, "voltage": 0, "util_pct": 0})
 
     def __init__(self, *args, **kwargs):
@@ -176,30 +202,31 @@
     def compose(self) -> ComposeResult:
         yield Horizontal(Label("[underline]Clocks"),
                          Label("", classes="statvalue"))
         yield Horizontal(Label("  GPU core:",),
                          Label("", id="clk_core_val", classes="statvalue"))
         yield Horizontal(Label("  Memory:"),
                          Label("", id="clk_memory_val", classes="statvalue"))
-        yield Horizontal(Label(""), Label("", classes="statvalue"))  # padding to split groups
+        # padding to split groups
+        yield Horizontal(Label(""), Label("", classes="statvalue"))
         yield Horizontal(Label("[underline]Core"),
                          Label("", classes="statvalue"))
         yield Horizontal(Label("  Utilization:",),
                          Label("", id="util_pct", classes="statvalue"))
         yield Horizontal(Label("  Voltage:",),
                          Label("", id="clk_voltage_val", classes="statvalue"))
 
     def on_mount(self) -> None:
         """Event handler called when widget is added to the app."""
         self.timer_clocks = self.set_interval(1, self.update_core_vals)
 
     def update_core_vals(self) -> None:
         """Method to update GPU clock values to the current measurements.
         Run by a timer created 'on_mount'"""
-        self.core_vals = get_core_stats()
+        self.core_vals = get_core_stats(CARD)
 
     def watch_core_vals(self, core_vals: dict) -> None:
         """Called when the clocks attribute changes
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
         self.query_one("#clk_core_val",
                        Static).update(f"{format_frequency(core_vals['sclk'])}")
@@ -210,61 +237,63 @@
         self.query_one("#clk_memory_val",
                        Static).update(f"{format_frequency(core_vals['mclk'])}")
 
 
 class PowerDisplay(Static):
     """A widget to display GPU power stats."""
 
-    micro_watts = reactive({"limit": 0,
-                            "average": 0,
-                            "capability": 0,
-                            "default": 0})
+    watts = reactive({"limit": 0,
+                      "average": 0,
+                      "capability": 0,
+                      "default": 0})
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.timer_micro_watts = None
+        self.timer_watts = None
 
     def compose(self) -> ComposeResult:
         yield Horizontal(Label("[underline]Power"),
                          Label("", classes="statvalue"))
         yield Horizontal(Label("  Usage:",),
                          Label("", id="pwr_avg_val", classes="statvalue"))
-        yield Horizontal(Label(""), Label("", classes="statvalue"))  # padding to split groups
+        # padding to split groups
+        yield Horizontal(Label(""), Label("", classes="statvalue"))
         yield Horizontal(Label("[underline]Limits"),
                          Label("", classes="statvalue"))
         yield Horizontal(Label("  Configured:",),
                          Label("", id="pwr_lim_val", classes="statvalue"))
         yield Horizontal(Label("  Default:",),
                          Label("", id="pwr_def_val", classes="statvalue"))
         yield Horizontal(Label("  Board capability:",),
                          Label("", id="pwr_cap_val", classes="statvalue"))
 
     def on_mount(self) -> None:
         """Event handler called when widget is added to the app."""
-        self.timer_micro_watts = self.set_interval(1, self.update_micro_watts)
+        self.timer_watts = self.set_interval(1, self.update_watts)
 
-    def update_micro_watts(self) -> None:
+    def update_watts(self) -> None:
         """Method to update GPU power values to current measurements.
 
         Run by a timer created 'on_mount'"""
-        self.micro_watts = get_power_stats()
+        self.watts = get_power_stats(CARD)
 
-    def watch_micro_watts(self, micro_watts: dict) -> None:
-        """Called when the micro_watts attributes change.
+    def watch_watts(self, watts: dict) -> None:
+        """Called when the 'watts' reactive attribute (var) changes.
          - Updates label values
          - Casting inputs to string to avoid type problems w/ int/None"""
         self.query_one("#pwr_avg_val",
-                       Static).update(f"{micro_watts['average']}W")
+                       Static).update(f"{watts['average']}W")
         self.query_one("#pwr_lim_val",
-                       Static).update(f"{micro_watts['limit']}W")
+                       Static).update(f"{watts['limit']}W")
         self.query_one("#pwr_def_val",
-                       Static).update(f"{micro_watts['default']}W")
+                       Static).update(f"{watts['default']}W")
         self.query_one("#pwr_cap_val",
-                       Static).update(f"{micro_watts['capability']}W")
+                       Static).update(f"{watts['capability']}W")
 
 
 def tui() -> None:
     '''Spawns the textual UI only during CLI invocation / after argparse'''
-    if CARD is None:
+    if len(AMDGPU_CARDS) > 0:
+        app = GPUStats()
+        app.run()
+    else:
         sys.exit('Could not find an AMD GPU, exiting.')
-    app = GPUStats()
-    app.run()
```

### Comparing `amdgpu_stats-0.1.8/setup.py` & `amdgpu_stats-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 ['humanfriendly>=10.0', 'textual>=0.10']
 
 entry_points = \
 {'console_scripts': ['amdgpu-stats = amdgpu_stats.interface:tui']}
 
 setup_kwargs = {
     'name': 'amdgpu-stats',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'A simple module/TUI (using Textual) that provides AMD GPU statistics',
-    'long_description': '# amdgpu_stats\n\nA simple Python module/TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics\n\n![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")\n\n![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")\n\nThe GPU and temperature nodes (`edge`/`junction`/etc.) are discovered automatically.\n\nStatistics are not logged; only toggling Dark/light mode and the stat names / source files.\n\nTested _only_ on `RX6000` series cards; APUs and more _may_ be supported. Please file an issue if finding incompatibility!\n\n## Requirements\nOnly `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.\n\nIt _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.\n\nThis is assumed present for *control* over the elements being monitored. Untested without. \n\nSee [this Arch Wiki entry](https://wiki.archlinux.org/title/AMDGPU#Boot_parameter) for context.\n\n## Installation / Usage\n```\npip install amdgpu-stats\n```\nOnce installed, run `amdgpu-stats` in your terminal of choice\n\n## Module\n\n*Rudimentary* support as a module exists; functions / variables offered can be found in `amdgpu_stats.utils`\n\nDemonstration:\n```\nIn [1]: import amdgpu_stats.utils\n\nIn [2]: print(amdgpu_stats.utils.get_core_stats())\n{\'sclk\': 0, \'mclk\': 1000000000, \'voltage\': 0.01, \'util_pct\': 0}\n\nIn [3]: print(amdgpu_stats.utils.get_power_stats())\n{\'limit\': 281, \'average\': 35, \'capability\': 323, \'default\': 281}\n\nIn [4]: print(amdgpu_stats.utils.get_temp_stats())\n{\'edge\': 33, \'junction\': 36, \'mem\': 42}\n\nIn [5]: print(amdgpu_stats.utils.get_fan_stats())\n{\'fan_rpm\': 0, \'fan_rpm_target\': 0}\n```\n## Documentation\n\nFor more information on the module, see:\n - `help(\'amdgpu_stats.utils\')` in your interpreter\n - [ReadTheDocs](https://amdgpu-stats.readthedocs.io/en/latest/)\n - [the module source](https://github.com/joshlay/amdgpu_stats/blob/master/src/amdgpu_stats/utils.py) for more info\n',
+    'long_description': '# amdgpu_stats\n\nA simple Python module/TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics\n\n![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")\n\nThe GPU and temperature nodes (`edge`/`junction`/etc.) are discovered automatically.\n\nPlease see [the module section](#module) or [the docs](https://amdgpu-stats.readthedocs.io/en/latest/) for information on usage as an `import` in other tooling\n\nTested _only_ on `RX6000` series cards; APUs and more _may_ be supported. Please file an issue if finding incompatibility!\n\n## Requirements\nOnly `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.\n\nIt _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.\n\nThis is assumed present for *control* over the elements being monitored. Untested without. \n\nSee [this Arch Wiki entry](https://wiki.archlinux.org/title/AMDGPU#Boot_parameter) for context.\n\n## Installation / Usage\n```\npip install amdgpu-stats\n```\nOnce installed, run `amdgpu-stats` in your terminal of choice\n\n## Module\n\n*Rudimentary* support as a module exists; functions / variables offered can be found in `amdgpu_stats.utils`\n\nDemonstration:\n```\nIn [1]: import amdgpu_stats.utils\n\nIn [2]: amdgpu_stats.utils.AMDGPU_CARDS\nOut[2]: {\'card0\': \'/sys/class/drm/card0/device/hwmon/hwmon9\'}\n\nIn [3]: amdgpu_stats.utils.get_core_stats(\'card0\')\nOut[3]: {\'sclk\': 640000000, \'mclk\': 1000000000, \'voltage\': 0.79, \'util_pct\': 65}\n\nIn [4]: amdgpu_stats.utils.get_clock(\'card0\', \'core\', format_freq=True)\nOut[4]: \'659 MHz\' \n```\nFeature requests [are encouraged](https://github.com/joshlay/amdgpu_stats/issues) :)\n\n## Documentation\n\nFor more information on the module, see:\n - `help(\'amdgpu_stats.utils\')` in your interpreter\n - [ReadTheDocs](https://amdgpu-stats.readthedocs.io/en/latest/)\n - [the module source](https://github.com/joshlay/amdgpu_stats/blob/master/src/amdgpu_stats/utils.py) for more info\n',
     'author': 'Josh Lay',
     'author_email': 'pypi@jlay.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/joshlay/amdgpu_stats',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `amdgpu_stats-0.1.8/PKG-INFO` & `amdgpu_stats-0.1.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amdgpu-stats
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple module/TUI (using Textual) that provides AMD GPU statistics
 Home-page: https://github.com/joshlay/amdgpu_stats
 License: MIT
 Author: Josh Lay
 Author-email: pypi@jlay.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,19 +20,17 @@
 
 # amdgpu_stats
 
 A simple Python module/TUI _(using [Textual](https://textual.textualize.io/))_ that shows AMD GPU statistics
 
 ![Screenshot of main screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/main.png "Main screen")
 
-![Screenshot of log screen](https://raw.githubusercontent.com/joshlay/amdgpu_stats/master/screens/logging.png "Logging screen")
-
 The GPU and temperature nodes (`edge`/`junction`/etc.) are discovered automatically.
 
-Statistics are not logged; only toggling Dark/light mode and the stat names / source files.
+Please see [the module section](#module) or [the docs](https://amdgpu-stats.readthedocs.io/en/latest/) for information on usage as an `import` in other tooling
 
 Tested _only_ on `RX6000` series cards; APUs and more _may_ be supported. Please file an issue if finding incompatibility!
 
 ## Requirements
 Only `Linux` is supported. Information is _completely_ sourced from interfaces in `sysfs`.
 
 It _may_ be necessary to update the `amdgpu.ppfeaturemask` parameter to enable metrics.
@@ -51,26 +49,25 @@
 
 *Rudimentary* support as a module exists; functions / variables offered can be found in `amdgpu_stats.utils`
 
 Demonstration:
 ```
 In [1]: import amdgpu_stats.utils
 
-In [2]: print(amdgpu_stats.utils.get_core_stats())
-{'sclk': 0, 'mclk': 1000000000, 'voltage': 0.01, 'util_pct': 0}
-
-In [3]: print(amdgpu_stats.utils.get_power_stats())
-{'limit': 281, 'average': 35, 'capability': 323, 'default': 281}
+In [2]: amdgpu_stats.utils.AMDGPU_CARDS
+Out[2]: {'card0': '/sys/class/drm/card0/device/hwmon/hwmon9'}
 
-In [4]: print(amdgpu_stats.utils.get_temp_stats())
-{'edge': 33, 'junction': 36, 'mem': 42}
+In [3]: amdgpu_stats.utils.get_core_stats('card0')
+Out[3]: {'sclk': 640000000, 'mclk': 1000000000, 'voltage': 0.79, 'util_pct': 65}
 
-In [5]: print(amdgpu_stats.utils.get_fan_stats())
-{'fan_rpm': 0, 'fan_rpm_target': 0}
+In [4]: amdgpu_stats.utils.get_clock('card0', 'core', format_freq=True)
+Out[4]: '659 MHz' 
 ```
+Feature requests [are encouraged](https://github.com/joshlay/amdgpu_stats/issues) :)
+
 ## Documentation
 
 For more information on the module, see:
  - `help('amdgpu_stats.utils')` in your interpreter
  - [ReadTheDocs](https://amdgpu-stats.readthedocs.io/en/latest/)
  - [the module source](https://github.com/joshlay/amdgpu_stats/blob/master/src/amdgpu_stats/utils.py) for more info
```

