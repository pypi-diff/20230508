# Comparing `tmp/truckersmp-cli-0.9.1.tar.gz` & `tmp/truckersmp-cli-0.9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truckersmp-cli-0.9.1.tar", last modified: Wed Apr 20 13:18:21 2022, max compression
+gzip compressed data, was "truckersmp-cli-0.9.1.1.tar", last modified: Wed Apr 20 13:47:22 2022, max compression
```

## Comparing `truckersmp-cli-0.9.1.tar` & `truckersmp-cli-0.9.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 13:18:21.526046 truckersmp-cli-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    23514 2022-04-20 13:18:21.526046 truckersmp-cli-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22623 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/RELEASE
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-04-20 13:18:21.526046 truckersmp-cli-0.9.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)      148 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      344 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp-cli
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 13:18:21.526046 truckersmp-cli-0.9.1/truckersmp_cli/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15414 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/args.py
--rw-r--r--   0 runner    (1001) docker     (121)    12647 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2191 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/flatpak_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    16937 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/gamestarter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/proton.json
--rw-r--r--   0 runner    (1001) docker     (121)     9589 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/steamcmd.py
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/steamruntime.json
--rwxr-xr-x   0 runner    (1001) docker     (121)     4362 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/steamruntime_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20992 2022-04-20 13:18:11.000000 truckersmp-cli-0.9.1/truckersmp_cli/truckersmp-cli.exe
--rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/truckersmp.py
--rw-r--r--   0 runner    (1001) docker     (121)    31149 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-04-20 13:17:41.000000 truckersmp-cli-0.9.1/truckersmp_cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 13:18:21.526046 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23514 2022-04-20 13:18:21.000000 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-04-20 13:18:21.000000 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 13:18:21.000000 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 13:18:21.000000 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-20 13:18:21.000000 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-20 13:18:21.000000 truckersmp-cli-0.9.1/truckersmp_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 13:47:22.468110 truckersmp-cli-0.9.1.1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       70 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    23576 2022-04-20 13:47:22.468110 truckersmp-cli-0.9.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    22683 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/RELEASE
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-04-20 13:47:22.468110 truckersmp-cli-0.9.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)      148 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      344 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp-cli
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 13:47:22.464110 truckersmp-cli-0.9.1.1/truckersmp_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15587 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/args.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12879 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2191 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/flatpak_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16937 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/gamestarter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6401 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/proton.json
+-rw-r--r--   0 runner    (1001) docker     (121)     9589 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/steamcmd.py
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/steamruntime.json
+-rwxr-xr-x   0 runner    (1001) docker     (121)     4362 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/steamruntime_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    20992 2022-04-20 13:47:10.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/truckersmp-cli.exe
+-rw-r--r--   0 runner    (1001) docker     (121)     4162 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/truckersmp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31149 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4322 2022-04-20 13:46:43.000000 truckersmp-cli-0.9.1.1/truckersmp_cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 13:47:22.468110 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    23576 2022-04-20 13:47:22.000000 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2022-04-20 13:47:22.000000 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 13:47:22.000000 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 13:47:22.000000 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2022-04-20 13:47:22.000000 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-04-20 13:47:22.000000 truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/top_level.txt
```

### Comparing `truckersmp-cli-0.9.1/LICENSE` & `truckersmp-cli-0.9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/PKG-INFO` & `truckersmp-cli-0.9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truckersmp-cli
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: A simple launcher for TruckersMP to be used with Wine/Proton
 Home-page: https://github.com/truckersmp-cli/truckersmp-cli
 License: MIT
 Project-URL: Bug Tracker, https://github.com/truckersmp-cli/truckersmp-cli/issues
 Project-URL: Source Code, https://github.com/truckersmp-cli/truckersmp-cli
 Platform: x86_64 POSIX systems
 Classifier: Development Status :: 3 - Alpha
@@ -102,14 +102,15 @@
 ## Options
 
 Short option|Long option|Description
 ---|---|---
 `-h`|`--help`|Show help
 `-b VERSION`|`--beta VERSION`|Set game version to VERSION, useful for downgrading (e.g. `temporary_1_35`)
 `-c FILE`|`--configfile FILE`|Use alternative configuration file<br><br>Default: `$XDG_CONFIG_HOME/truckersmp-cli/truckersmp-cli.conf`
+`-d`|`--enable-d3d11`|**DEPRECATED** Use Direct3D 11 instead of OpenGL
 `-f`|`--flatpak-steam`|Use Flatpak version of Steam with Proton<br><br>Note: Currently Steam Runtime is not supported and will be disabled
 `-g DIR`|`--gamedir DIR`|Choose a different directory for the game files<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/(Game name)/data`
 `-i APPID`|`--proton-appid APPID`|Choose a different AppID or version name ("X.Y" format) of Proton (Needs an update for changes)
 `-l LOG`|`--logfile LOG`|Write log into LOG, `-vv` option is recommended<br><br>Default: Empty string (only stderr)<br>Note: Messages from Steam/SteamCMD won't be written, only from this script<br>See [#game-logs](https://github.com/truckersmp-cli/truckersmp-cli#game-logs) for game log locations.
 `-m DIR`|`--moddir DIR`|Choose a different directory for the mod files<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/TruckersMP`
 `-n NAME`|`--account NAME`|Steam account name to use
 `-o DIR`|`--protondir DIR`|Choose a different Proton directory<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/Proton`
@@ -253,15 +254,15 @@
 ### Direct3D 11 (DXVK or wined3d)
 
 * Faster than OpenGL when DXVK is used.
     * DXVK requires Vulkan support.
     * DXVK 1.4.6 or newer is needed because older versions have rendering issue. If you're using Proton, use 4.11-10 or newer.
 * Proton uses DXVK by default.
     * When using Proton, wined3d can be used by specifying `--use-wined3d`, but it's not recommended because this is slower than OpenGL.
-* Used only when `-r dx11` or `--rendering-backend dx11` is given.
+* Used only when `-d` or `--enable-d3d11` is specified.
 
 ## Configuration file
 
 It's possible to set various game settings and third party programs in a configuration file.
 
 The configuration file format is similar to the INI format known from Windows with several sections `[section]` containing key-value-pairs `key = value`.
 All sections are optional and a key-value-pair has to be in a section.
```

### Comparing `truckersmp-cli-0.9.1/README.md` & `truckersmp-cli-0.9.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 ## Options
 
 Short option|Long option|Description
 ---|---|---
 `-h`|`--help`|Show help
 `-b VERSION`|`--beta VERSION`|Set game version to VERSION, useful for downgrading (e.g. `temporary_1_35`)
 `-c FILE`|`--configfile FILE`|Use alternative configuration file<br><br>Default: `$XDG_CONFIG_HOME/truckersmp-cli/truckersmp-cli.conf`
+`-d`|`--enable-d3d11`|**DEPRECATED** Use Direct3D 11 instead of OpenGL
 `-f`|`--flatpak-steam`|Use Flatpak version of Steam with Proton<br><br>Note: Currently Steam Runtime is not supported and will be disabled
 `-g DIR`|`--gamedir DIR`|Choose a different directory for the game files<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/(Game name)/data`
 `-i APPID`|`--proton-appid APPID`|Choose a different AppID or version name ("X.Y" format) of Proton (Needs an update for changes)
 `-l LOG`|`--logfile LOG`|Write log into LOG, `-vv` option is recommended<br><br>Default: Empty string (only stderr)<br>Note: Messages from Steam/SteamCMD won't be written, only from this script<br>See [#game-logs](https://github.com/truckersmp-cli/truckersmp-cli#game-logs) for game log locations.
 `-m DIR`|`--moddir DIR`|Choose a different directory for the mod files<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/TruckersMP`
 `-n NAME`|`--account NAME`|Steam account name to use
 `-o DIR`|`--protondir DIR`|Choose a different Proton directory<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/Proton`
@@ -231,15 +232,15 @@
 ### Direct3D 11 (DXVK or wined3d)
 
 * Faster than OpenGL when DXVK is used.
     * DXVK requires Vulkan support.
     * DXVK 1.4.6 or newer is needed because older versions have rendering issue. If you're using Proton, use 4.11-10 or newer.
 * Proton uses DXVK by default.
     * When using Proton, wined3d can be used by specifying `--use-wined3d`, but it's not recommended because this is slower than OpenGL.
-* Used only when `-r dx11` or `--rendering-backend dx11` is given.
+* Used only when `-d` or `--enable-d3d11` is specified.
 
 ## Configuration file
 
 It's possible to set various game settings and third party programs in a configuration file.
 
 The configuration file format is similar to the INI format known from Windows with several sections `[section]` containing key-value-pairs `key = value`.
 All sections are optional and a key-value-pair has to be in a section.
```

### Comparing `truckersmp-cli-0.9.1/setup.cfg` & `truckersmp-cli-0.9.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/args.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,18 @@
                 [Default: $XDG_CONFIG_HOME/truckersmp-cli/truckersmp-cli.conf]"""))
     store_actions.append(parser.add_argument(
         "--download-throttle", metavar="SPEED", type=int,
         default=-1,
         help="""limit download speed to SPEED (KiB/s),
                 disabled if negative value is specified [Default: -1]"""))
     store_actions.append(parser.add_argument(
+        "-d", "--enable-d3d11",
+        help="**DEPRECATED** use Direct3D 11 instead of OpenGL",
+        action="store_true"))
+    store_actions.append(parser.add_argument(
         "-f", "--flatpak-steam",
         default=None,
         help="""use Flatpak version of Steam with Proton
                 Note: Currently Steam Runtime is not supported and will be disabled""",
         action="store_true"))
     store_actions.append(parser.add_argument(
         "-g", "--gamedir", metavar="DIR",
```

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/configfile.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/configfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,19 @@
             raise ValueError(
                 ConfigFile.format_error("without-rich-presence", ex)) from ex
 
     def _determine_rendering_backend(self):
         """Determine rendering backend."""
         config_src = ConfigSource.OPTION
 
+        if Args.enable_d3d11:
+            logging.warning("'--enable-d3d11' ('-d') option is deprecated,"
+                            " use '--rendering-backend dx11 (-r dx11)' instead")
+            Args.rendering_backend = "dx11"
+
         if Args.rendering_backend == "auto":
             rendering_backend = None
             try:
                 if Args.game in self._parser:
                     rendering_backend = self._parser[Args.game].get("rendering-backend")
                 # use OpenGL when "rendering-backend" is not specified
                 # in the game specific section
```

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/flatpak_helper.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/flatpak_helper.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/gamestarter.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/gamestarter.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/logger.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/logger.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/main.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/main.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/steamcmd.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/steamcmd.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/steamruntime_helper.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/steamruntime_helper.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/truckersmp-cli.exe` & `truckersmp-cli-0.9.1.1/truckersmp_cli/truckersmp-cli.exe`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/truckersmp.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/truckersmp.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/utils.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/utils.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli/variables.py` & `truckersmp-cli-0.9.1.1/truckersmp_cli/variables.py`

 * *Files identical despite different names*

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli.egg-info/PKG-INFO` & `truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truckersmp-cli
-Version: 0.9.1
+Version: 0.9.1.1
 Summary: A simple launcher for TruckersMP to be used with Wine/Proton
 Home-page: https://github.com/truckersmp-cli/truckersmp-cli
 License: MIT
 Project-URL: Bug Tracker, https://github.com/truckersmp-cli/truckersmp-cli/issues
 Project-URL: Source Code, https://github.com/truckersmp-cli/truckersmp-cli
 Platform: x86_64 POSIX systems
 Classifier: Development Status :: 3 - Alpha
@@ -102,14 +102,15 @@
 ## Options
 
 Short option|Long option|Description
 ---|---|---
 `-h`|`--help`|Show help
 `-b VERSION`|`--beta VERSION`|Set game version to VERSION, useful for downgrading (e.g. `temporary_1_35`)
 `-c FILE`|`--configfile FILE`|Use alternative configuration file<br><br>Default: `$XDG_CONFIG_HOME/truckersmp-cli/truckersmp-cli.conf`
+`-d`|`--enable-d3d11`|**DEPRECATED** Use Direct3D 11 instead of OpenGL
 `-f`|`--flatpak-steam`|Use Flatpak version of Steam with Proton<br><br>Note: Currently Steam Runtime is not supported and will be disabled
 `-g DIR`|`--gamedir DIR`|Choose a different directory for the game files<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/(Game name)/data`
 `-i APPID`|`--proton-appid APPID`|Choose a different AppID or version name ("X.Y" format) of Proton (Needs an update for changes)
 `-l LOG`|`--logfile LOG`|Write log into LOG, `-vv` option is recommended<br><br>Default: Empty string (only stderr)<br>Note: Messages from Steam/SteamCMD won't be written, only from this script<br>See [#game-logs](https://github.com/truckersmp-cli/truckersmp-cli#game-logs) for game log locations.
 `-m DIR`|`--moddir DIR`|Choose a different directory for the mod files<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/TruckersMP`
 `-n NAME`|`--account NAME`|Steam account name to use
 `-o DIR`|`--protondir DIR`|Choose a different Proton directory<br><br>Default: `$XDG_DATA_HOME/truckersmp-cli/Proton`
@@ -253,15 +254,15 @@
 ### Direct3D 11 (DXVK or wined3d)
 
 * Faster than OpenGL when DXVK is used.
     * DXVK requires Vulkan support.
     * DXVK 1.4.6 or newer is needed because older versions have rendering issue. If you're using Proton, use 4.11-10 or newer.
 * Proton uses DXVK by default.
     * When using Proton, wined3d can be used by specifying `--use-wined3d`, but it's not recommended because this is slower than OpenGL.
-* Used only when `-r dx11` or `--rendering-backend dx11` is given.
+* Used only when `-d` or `--enable-d3d11` is specified.
 
 ## Configuration file
 
 It's possible to set various game settings and third party programs in a configuration file.
 
 The configuration file format is similar to the INI format known from Windows with several sections `[section]` containing key-value-pairs `key = value`.
 All sections are optional and a key-value-pair has to be in a section.
```

### Comparing `truckersmp-cli-0.9.1/truckersmp_cli.egg-info/SOURCES.txt` & `truckersmp-cli-0.9.1.1/truckersmp_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

