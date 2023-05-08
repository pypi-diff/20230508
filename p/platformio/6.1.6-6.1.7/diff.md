# Comparing `tmp/platformio-6.1.6.tar.gz` & `tmp/platformio-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "platformio-6.1.6.tar", last modified: Mon Jan 23 11:41:36 2023, max compression
+gzip compressed data, was "platformio-6.1.7.tar", last modified: Mon May  8 14:59:21 2023, max compression
```

## Comparing `platformio-6.1.6.tar` & `platformio-6.1.7.tar`

### file list

```diff
@@ -1,358 +1,368 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.919365 platformio-6.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-01-23 11:28:43.000000 platformio-6.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-01-23 11:41:36.919365 platformio-6.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-01-23 11:28:43.000000 platformio-6.1.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.819365 platformio-6.1.6/platformio/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.823365 platformio-6.1.6/platformio/account/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.827365 platformio-6.1.6/platformio/account/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/forgot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/login.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/logout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/commands/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.827365 platformio-6.1.6/platformio/account/org/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.827365 platformio-6.1.6/platformio/account/org/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/org/commands/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.831365 platformio-6.1.6/platformio/account/team/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.831365 platformio-6.1.6/platformio/account/team/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/destroy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/team/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/account/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.791365 platformio-6.1.6/platformio/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.831365 platformio-6.1.6/platformio/assets/system/
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/system/99-platformio-udev.rules
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.791365 platformio-6.1.6/platformio/assets/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.795365 platformio-6.1.6/platformio/assets/templates/ide-projects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.835365 platformio-6.1.6/platformio/assets/templates/ide-projects/atom/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/atom/.clang_complete.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/atom/.gcc-flags.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/atom/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.835365 platformio-6.1.6/platformio/assets/templates/ide-projects/clion/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/clion/.gitignore.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/clion/CMakeLists.txt.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/clion/CMakeListsPrivate.txt.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.835365 platformio-6.1.6/platformio/assets/templates/ide-projects/codeblocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/codeblocks/platformio.cbp.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.835365 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/
--rw-r--r--   0 runner    (1001) docker     (123)    20663 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.cproject.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.project.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.835365 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.839365 platformio-6.1.6/platformio/assets/templates/ide-projects/emacs/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/emacs/.ccls.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/emacs/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.839365 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/.gitignore.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/Makefile.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/platformio.cflags.tpl
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/platformio.config.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/platformio.creator.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/platformio.cxxflags.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/platformio.files.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/qtcreator/platformio.includes.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.843365 platformio-6.1.6/platformio/assets/templates/ide-projects/sublimetext/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/sublimetext/.ccls.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/sublimetext/platformio.sublime-project.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.843365 platformio-6.1.6/platformio/assets/templates/ide-projects/vim/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/vim/.ccls.tpl
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/vim/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.843365 platformio-6.1.6/platformio/assets/templates/ide-projects/visualstudio/
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.filters.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.843365 platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.gitignore.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.843365 platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.847365 platformio-6.1.6/platformio/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.851365 platformio-6.1.6/platformio/builder/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/compilation_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/pioasm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piobuild.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piohooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/pioino.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piointegration.py
--rw-r--r--   0 runner    (1001) docker     (123)    42396 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piolib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piomaxlen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piomisc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/pioplatform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/pioproject.py
--rw-r--r--   0 runner    (1001) docker     (123)     8102 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piosize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piotarget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/piotest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/builder/tools/pioupload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.855365 platformio-6.1.6/platformio/check/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/defect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.855365 platformio-6.1.6/platformio/check/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/tools/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/tools/clangtidy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9275 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/tools/cppcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/check/tools/pvsstudio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.859365 platformio-6.1.6/platformio/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/boards.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/ci.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.859365 platformio-6.1.6/platformio/commands/device/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16058 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/commands/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.859365 platformio-6.1.6/platformio/debug/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.863365 platformio-6.1.6/platformio/debug/config/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8857 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/blackmagic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/jlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/mspdebug.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/native.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/qemu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/config/renode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.863365 platformio-6.1.6/platformio/debug/process/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/process/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/process/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/process/gdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/debug/process/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.863365 platformio-6.1.6/platformio/device/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8573 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.867365 platformio-6.1.6/platformio/device/list/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/list/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/list/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.867365 platformio-6.1.6/platformio/device/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.871365 platformio-6.1.6/platformio/device/monitor/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/filters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/filters/hexlify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/filters/log2file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/filters/send_on_enter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/filters/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/device/monitor/terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.871365 platformio-6.1.6/platformio/home/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.871365 platformio-6.1.6/platformio/home/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.871365 platformio-6.1.6/platformio/home/rpc/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/ide.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4956 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/os.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/piocore.py
--rw-r--r--   0 runner    (1001) docker     (123)    12940 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/handlers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/rpc/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/home/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7383 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9309 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/maintenance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.875365 platformio-6.1.6/platformio/package/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.879365 platformio-6.1.6/platformio/package/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/outdated.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     8400 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/unpublish.py
--rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/lockfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.891365 platformio-6.1.6/platformio/package/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_download.py
--rw-r--r--   0 runner    (1001) docker     (123)    10483 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_symlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_uninstall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    11676 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/platform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manager/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.891365 platformio-6.1.6/platformio/package/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24640 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manifest/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/manifest/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15967 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/vcsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/package/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.895365 platformio-6.1.6/platformio/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/_packages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6585 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/platform/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/proc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.899365 platformio-6.1.6/platformio/project/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.899365 platformio-6.1.6/platformio/project/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/commands/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11614 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/commands/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/commands/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    16551 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.899365 platformio-6.1.6/platformio/project/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6433 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/integration/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    31481 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/project/savedeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/public.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.899365 platformio-6.1.6/platformio/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.899365 platformio-6.1.6/platformio/registry/access/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.903365 platformio-6.1.6/platformio/registry/access/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/commands/grant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/commands/private.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/commands/public.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/commands/revoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/access/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/registry/mirror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.903365 platformio-6.1.6/platformio/remote/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.903365 platformio-6.1.6/platformio/remote/ac/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/ac/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/ac/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/ac/psync.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/ac/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11782 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.907365 platformio-6.1.6/platformio/remote/client/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/agent_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/agent_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/async_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/device_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/device_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/run_or_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/client/update_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.907365 platformio-6.1.6/platformio/remote/factory/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/factory/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/factory/ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/remote/projectsync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.907365 platformio-6.1.6/platformio/run/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/run/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/run/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/run/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.911365 platformio-6.1.6/platformio/system/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.911365 platformio-6.1.6/platformio/system/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/commands/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/commands/prune.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/system/prune.py
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.915365 platformio-6.1.6/platformio/test/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.915365 platformio-6.1.6/platformio/test/reports/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/reports/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/reports/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/reports/junit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/reports/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.919365 platformio-6.1.6/platformio/test/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/googletest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.919365 platformio-6.1.6/platformio/test/runners/readers/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/readers/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/readers/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/test/runners/unity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-01-23 11:28:43.000000 platformio-6.1.6/platformio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 11:41:36.819365 platformio-6.1.6/platformio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-01-23 11:41:36.000000 platformio-6.1.6/platformio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-01-23 11:41:36.000000 platformio-6.1.6/platformio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 11:41:36.000000 platformio-6.1.6/platformio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-01-23 11:41:36.000000 platformio-6.1.6/platformio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-23 11:41:36.000000 platformio-6.1.6/platformio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-23 11:41:36.000000 platformio-6.1.6/platformio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 11:41:36.919365 platformio-6.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3392 2023-01-23 11:28:43.000000 platformio-6.1.6/setup.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.300732 platformio-6.1.7/
+-rw-r--r--   0 ikravets   (501) staff       (20)     9169 2019-12-19 09:45:48.000000 platformio-6.1.7/LICENSE
+-rw-r--r--   0 ikravets   (501) staff       (20)     6549 2023-05-08 14:59:21.300299 platformio-6.1.7/PKG-INFO
+-rw-r--r--   0 ikravets   (501) staff       (20)     5122 2022-08-12 13:55:00.000000 platformio-6.1.7/README.rst
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.038491 platformio-6.1.7/platformio/
+-rw-r--r--   0 ikravets   (501) staff       (20)     2101 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4606 2022-10-31 20:40:30.000000 platformio-6.1.7/platformio/__main__.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.045479 platformio-6.1.7/platformio/account/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1593 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/cli.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    11093 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/client.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.051709 platformio-6.1.7/platformio/account/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1246 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/destroy.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1039 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/forgot.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1036 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/login.py
+-rw-r--r--   0 ikravets   (501) staff       (20)      879 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/logout.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1086 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/password.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1702 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/register.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4263 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/show.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1255 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/token.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2282 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/commands/update.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.053207 platformio-6.1.7/platformio/account/org/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1267 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.057801 platformio-6.1.7/platformio/account/org/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1089 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/add.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1305 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/create.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1194 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/destroy.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1666 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/list.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1100 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/org/commands/remove.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1804 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/org/commands/update.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.059307 platformio-6.1.7/platformio/account/team/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1287 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.067146 platformio-6.1.7/platformio/account/team/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1324 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/add.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1289 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/team/commands/create.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1388 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/destroy.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2181 2023-03-07 04:32:55.000000 platformio-6.1.7/platformio/account/team/commands/list.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1327 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/account/team/commands/remove.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1809 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/team/commands/update.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2895 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/account/validate.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8083 2022-11-01 18:28:49.000000 platformio-6.1.7/platformio/app.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.005107 platformio-6.1.7/platformio/assets/
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.068239 platformio-6.1.7/platformio/assets/system/
+-rw-r--r--   0 ikravets   (501) staff       (20)     8260 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/system/99-platformio-udev.rules
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.005331 platformio-6.1.7/platformio/assets/templates/
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.009147 platformio-6.1.7/platformio/assets/templates/ide-projects/
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.074504 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/
+-rw-r--r--   0 ikravets   (501) staff       (20)      109 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.clang_complete.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      530 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.gcc-flags.json.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       37 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.gitignore.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.077481 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/
+-rw-r--r--   0 ikravets   (501) staff       (20)       43 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/.gitignore.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     1068 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeLists.txt.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     3885 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeListsPrivate.txt.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.078575 platformio-6.1.7/platformio/assets/templates/ide-projects/codeblocks/
+-rw-r--r--   0 ikravets   (501) staff       (20)     2565 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/codeblocks/platformio.cbp.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.082530 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/
+-rw-r--r--   0 ikravets   (501) staff       (20)    20663 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.cproject.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      817 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.project.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.085456 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/
+-rw-r--r--   0 ikravets   (501) staff       (20)     2838 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     2410 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      756 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.088166 platformio-6.1.7/platformio/assets/templates/ide-projects/emacs/
+-rw-r--r--   0 ikravets   (501) staff       (20)      176 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/emacs/.ccls.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       27 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/emacs/.gitignore.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.007159 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.090123 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/
+-rw-r--r--   0 ikravets   (501) staff       (20)     2520 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/configurations.xml.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.092719 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/
+-rw-r--r--   0 ikravets   (501) staff       (20)     2330 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/configurations.xml.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     2001 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/launcher.properties.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      481 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/private/private.xml.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      912 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/netbeans/nbproject/project.xml.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.097969 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/
+-rw-r--r--   0 ikravets   (501) staff       (20)       17 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/.gitignore.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      383 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/Makefile.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       52 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.cflags.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)      171 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.config.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       11 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.creator.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       53 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.cxxflags.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       75 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.files.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       65 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/qtcreator/platformio.includes.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.099201 platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/
+-rw-r--r--   0 ikravets   (501) staff       (20)      176 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/.ccls.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     2069 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/platformio.sublime-project.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.100288 platformio-6.1.7/platformio/assets/templates/ide-projects/vim/
+-rw-r--r--   0 ikravets   (501) staff       (20)      176 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vim/.ccls.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)       43 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vim/.gitignore.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.101472 platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/
+-rw-r--r--   0 ikravets   (501) staff       (20)      975 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.filters.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     3806 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.102102 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/
+-rw-r--r--   0 ikravets   (501) staff       (20)       94 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.gitignore.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.104130 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/
+-rw-r--r--   0 ikravets   (501) staff       (20)     3367 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     1159 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl
+-rw-r--r--   0 ikravets   (501) staff       (20)     2832 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.105355 platformio-6.1.7/platformio/builder/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/builder/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8228 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/main.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.116201 platformio-6.1.7/platformio/builder/tools/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-04-11 08:55:48.000000 platformio-6.1.7/platformio/builder/tools/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1027 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/pioasm.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    12577 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/piobuild.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1676 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piohooks.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8210 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/pioino.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6335 2022-11-01 18:28:49.000000 platformio-6.1.7/platformio/builder/tools/piointegration.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    42536 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/piolib.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2973 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piomaxlen.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4431 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piomisc.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8217 2023-04-24 14:16:09.000000 platformio-6.1.7/platformio/builder/tools/pioplatform.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1700 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/pioproject.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8102 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piosize.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3317 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/builder/tools/piotarget.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2106 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/piotest.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8472 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/builder/tools/pioupload.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5269 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/cache.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.118060 platformio-6.1.7/platformio/check/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/check/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    10813 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/cli.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3093 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/defect.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.121755 platformio-6.1.7/platformio/check/tools/
+-rw-r--r--   0 ikravets   (501) staff       (20)     1319 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/check/tools/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8710 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3094 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/clangtidy.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     9357 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/cppcheck.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8421 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/check/tools/pvsstudio.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3192 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.127329 platformio-6.1.7/platformio/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2824 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/boards.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5638 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/ci.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.128166 platformio-6.1.7/platformio/commands/device/
+-rw-r--r--   0 ikravets   (501) staff       (20)      750 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/commands/device/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    16025 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/lib.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    12882 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/commands/platform.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2477 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/commands/settings.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1244 2022-05-17 16:23:31.000000 platformio-6.1.7/platformio/commands/update.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4385 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/commands/upgrade.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3308 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/compat.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.130709 platformio-6.1.7/platformio/debug/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2021-10-25 08:38:45.000000 platformio-6.1.7/platformio/debug/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6037 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.136263 platformio-6.1.7/platformio/debug/config/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2021-10-25 08:38:45.000000 platformio-6.1.7/platformio/debug/config/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8861 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2074 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/blackmagic.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1766 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/debug/config/factory.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1098 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/generic.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1290 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/jlink.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1050 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/mspdebug.py
+-rw-r--r--   0 ikravets   (501) staff       (20)      966 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/native.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1091 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/qemu.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1285 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/config/renode.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1137 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/exception.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5063 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/helpers.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.139206 platformio-6.1.7/platformio/debug/process/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2021-10-25 08:38:45.000000 platformio-6.1.7/platformio/debug/process/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4893 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/process/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3461 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/debug/process/client.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     7370 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/process/gdb.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5656 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/debug/process/server.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.140918 platformio-6.1.7/platformio/device/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/device/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)      933 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/cli.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8573 2022-12-13 19:50:55.000000 platformio-6.1.7/platformio/device/finder.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.146328 platformio-6.1.7/platformio/device/list/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/list/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3333 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/list/command.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5476 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/device/list/util.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.148230 platformio-6.1.7/platformio/device/monitor/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6127 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/device/monitor/command.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.152433 platformio-6.1.7/platformio/device/monitor/filters/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3429 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1285 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/hexlify.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1547 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/device/monitor/filters/log2file.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1266 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/send_on_enter.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1386 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/device/monitor/filters/time.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6224 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/device/monitor/terminal.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3009 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/exception.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6767 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/fs.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.154787 platformio-6.1.7/platformio/home/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/home/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3405 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.155918 platformio-6.1.7/platformio/home/rpc/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/home/rpc/__init__.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.166147 platformio-6.1.7/platformio/home/rpc/handlers/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/home/rpc/handlers/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1196 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/account.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3122 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/app.py
+-rw-r--r--   0 ikravets   (501) staff       (20)      653 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2994 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/ide.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1966 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/misc.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5081 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/os.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     7644 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/piocore.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2261 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/platform.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    12206 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/project.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1280 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/handlers/registry.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4604 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/rpc/server.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4089 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/home/run.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     7394 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/http.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8953 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/maintenance.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.176488 platformio-6.1.7/platformio/package/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/package/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1778 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/package/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.187992 platformio-6.1.7/platformio/package/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/package/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3888 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/commands/exec.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    12338 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/install.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8182 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/list.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     7160 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/outdated.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1606 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/pack.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6995 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/publish.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2367 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/package/commands/search.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4841 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/commands/show.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8362 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/uninstall.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1656 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/package/commands/unpublish.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8643 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/commands/update.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5890 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/download.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2075 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/exception.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3580 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/lockfile.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.200785 platformio-6.1.7/platformio/package/manager/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/package/manager/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3875 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/_download.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    10482 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/_install.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2414 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manager/_legacy.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     7688 2022-08-12 13:55:00.000000 platformio-6.1.7/platformio/package/manager/_registry.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2642 2023-04-21 08:25:48.000000 platformio-6.1.7/platformio/package/manager/_symlink.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3211 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/package/manager/_uninstall.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4594 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manager/_update.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    11676 2023-04-15 15:52:33.000000 platformio-6.1.7/platformio/package/manager/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3081 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/core.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4369 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manager/library.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6312 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manager/platform.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1180 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/package/manager/tool.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.204077 platformio-6.1.7/platformio/package/manifest/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/package/manifest/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    24640 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/manifest/parser.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     9003 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/manifest/schema.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    15965 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/meta.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8488 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/package/pack.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6601 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/unpack.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8602 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/package/vcsclient.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1686 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/package/version.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.213259 platformio-6.1.7/platformio/platform/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2020-09-03 11:43:11.000000 platformio-6.1.7/platformio/platform/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3490 2023-04-22 10:47:04.000000 platformio-6.1.7/platformio/platform/_packages.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6830 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/platform/_run.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8687 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/platform/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5114 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/platform/board.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1380 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/platform/exception.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3311 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/platform/factory.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6466 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/proc.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.225961 platformio-6.1.7/platformio/project/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2019-12-19 09:45:48.000000 platformio-6.1.7/platformio/project/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1016 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/project/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.232507 platformio-6.1.7/platformio/project/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/project/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1955 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/commands/config.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    12843 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/commands/init.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2826 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/commands/metadata.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    17414 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/config.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1908 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/exception.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6529 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/helpers.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.235803 platformio-6.1.7/platformio/project/integration/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/project/integration/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6541 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/integration/generator.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    31475 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/project/options.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3077 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/project/savedeps.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1452 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/public.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.241993 platformio-6.1.7/platformio/registry/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/__init__.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.245501 platformio-6.1.7/platformio/registry/access/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1234 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.254110 platformio-6.1.7/platformio/registry/access/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1521 2023-04-18 19:02:58.000000 platformio-6.1.7/platformio/registry/access/commands/grant.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2134 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/list.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1241 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/private.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1238 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/public.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1424 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/commands/revoke.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1074 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/registry/access/validate.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5755 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/registry/client.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3748 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/registry/mirror.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.257619 platformio-6.1.7/platformio/remote/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/__init__.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.263307 platformio-6.1.7/platformio/remote/ac/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2635 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/ac/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1421 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/process.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2326 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/psync.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2108 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/ac/serial.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    11855 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.272670 platformio-6.1.7/platformio/remote/client/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/client/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1337 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/client/agent_list.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8904 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/remote/client/agent_service.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2306 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/async_base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6967 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1989 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/device_list.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     8410 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/device_monitor.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     9718 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/client/run_or_test.py
+-rw-r--r--   0 ikravets   (501) staff       (20)      923 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/client/update_core.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.275712 platformio-6.1.7/platformio/remote/factory/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/factory/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3549 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/remote/factory/client.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1485 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/remote/factory/ssl.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3879 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/remote/projectsync.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.278843 platformio-6.1.7/platformio/run/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/run/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     9788 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/run/cli.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1654 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/run/helpers.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3214 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/run/processor.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.281288 platformio-6.1.7/platformio/system/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1023 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/cli.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.283964 platformio-6.1.7/platformio/system/commands/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/commands/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2504 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/system/commands/completion.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2970 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/commands/info.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2306 2022-06-01 13:27:53.000000 platformio-6.1.7/platformio/system/commands/prune.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3281 2022-11-01 18:28:49.000000 platformio-6.1.7/platformio/system/completion.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3507 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/system/prune.py
+-rw-r--r--   0 ikravets   (501) staff       (20)    12460 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/telemetry.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.287700 platformio-6.1.7/platformio/test/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     6401 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/cli.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1144 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/exception.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2848 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/helpers.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.291940 platformio-6.1.7/platformio/test/reports/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     1237 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3681 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/test/reports/json.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4363 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/junit.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3703 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/reports/stdout.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4690 2023-01-23 11:01:56.000000 platformio-6.1.7/platformio/test/result.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.296548 platformio-6.1.7/platformio/test/runners/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/runners/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     7692 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/base.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3880 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/doctest.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2812 2022-07-09 16:11:32.000000 platformio-6.1.7/platformio/test/runners/factory.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     3679 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/googletest.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.298816 platformio-6.1.7/platformio/test/runners/readers/
+-rw-r--r--   0 ikravets   (501) staff       (20)      610 2022-05-16 11:22:08.000000 platformio-6.1.7/platformio/test/runners/readers/__init__.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     4692 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/readers/native.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     2751 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/readers/serial.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     9634 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/test/runners/unity.py
+-rw-r--r--   0 ikravets   (501) staff       (20)     5949 2023-05-08 14:58:34.000000 platformio-6.1.7/platformio/util.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.042236 platformio-6.1.7/platformio.egg-info/
+-rw-r--r--   0 ikravets   (501) staff       (20)     6549 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/PKG-INFO
+-rw-r--r--   0 ikravets   (501) staff       (20)    11636 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/SOURCES.txt
+-rw-r--r--   0 ikravets   (501) staff       (20)        1 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/dependency_links.txt
+-rw-r--r--   0 ikravets   (501) staff       (20)      136 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/entry_points.txt
+-rw-r--r--   0 ikravets   (501) staff       (20)      252 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/requires.txt
+-rw-r--r--   0 ikravets   (501) staff       (20)       11 2023-05-08 14:59:20.000000 platformio-6.1.7/platformio.egg-info/top_level.txt
+-rw-r--r--   0 ikravets   (501) staff       (20)       38 2023-05-08 14:59:21.300861 platformio-6.1.7/setup.cfg
+-rw-r--r--   0 ikravets   (501) staff       (20)     3600 2023-05-08 14:58:34.000000 platformio-6.1.7/setup.py
+drwxr-xr-x   0 ikravets   (501) staff       (20)        0 2023-05-08 14:59:21.299523 platformio-6.1.7/tests/
+-rw-r--r--   0 ikravets   (501) staff       (20)     3467 2023-05-08 14:58:34.000000 platformio-6.1.7/tests/test_examples.py
```

### Comparing `platformio-6.1.6/LICENSE` & `platformio-6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/PKG-INFO` & `platformio-6.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: platformio
-Version: 6.1.6
+Version: 6.1.7
 Summary: A professional collaborative platform for embedded development. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://platformio.org
 Author: PlatformIO Labs
 Author-email: contact@piolabs.com
 License: Apache Software License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -119,8 +118,7 @@
 
 The PlatformIO is licensed under the permissive Apache 2.0 license,
 so you can use it in both commercial and personal projects with confidence.
 
 .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
     :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
     :alt:  SWUbanner
-
```

### Comparing `platformio-6.1.6/README.rst` & `platformio-6.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/__init__.py` & `platformio-6.1.7/platformio/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
-
-VERSION = (6, 1, 6)
+VERSION = (6, 1, 7)
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "platformio"
 __description__ = (
     "A professional collaborative platform for embedded development. "
     "Cross-platform IDE and Unified Debugger. "
     "Static Code Analyzer and Remote Unit Testing. "
@@ -42,16 +40,16 @@
     "registry.platformio.org",
     "registry.nm1.platformio.org",
 ]
 __pioremote_endpoint__ = "ssl:host=remote.platformio.org:port=4413"
 
 __core_packages__ = {
     "contrib-piohome": "~3.4.2",
-    "contrib-pysite": "~2.%d%d.0" % (sys.version_info.major, sys.version_info.minor),
-    "tool-scons": "~4.40400.0",
+    "contrib-pioremote": "~1.0.0",
+    "tool-scons": "~4.40502.0",
     "tool-cppcheck": "~1.270.0",
     "tool-clangtidy": "~1.150005.0",
     "tool-pvs-studio": "~7.18.0",
 }
 
 __check_internet_hosts__ = [
     "185.199.110.153",  # Github.com
```

### Comparing `platformio-6.1.6/platformio/__main__.py` & `platformio-6.1.7/platformio/__main__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/__init__.py` & `platformio-6.1.7/platformio/account/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/cli.py` & `platformio-6.1.7/platformio/account/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/client.py` & `platformio-6.1.7/platformio/account/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,30 +17,26 @@
 
 from platformio import __accounts_api__, app
 from platformio.exception import PlatformioException
 from platformio.http import HTTPClient, HTTPClientError
 
 
 class AccountError(PlatformioException):
-
     MESSAGE = "{0}"
 
 
 class AccountNotAuthorized(AccountError):
-
     MESSAGE = "You are not authorized! Please log in to PlatformIO Account."
 
 
 class AccountAlreadyAuthorized(AccountError):
-
     MESSAGE = "You are already authorized with {0} account."
 
 
 class AccountClient(HTTPClient):  # pylint:disable=too-many-public-methods
-
     SUMMARY_CACHE_TTL = 60 * 60 * 24 * 7
 
     def __init__(self):
         super().__init__(__accounts_api__)
 
     @staticmethod
     def get_refresh_token():
@@ -294,15 +290,15 @@
             x_with_authorization=True,
         )
 
     def remove_org_owner(self, orgname, username):
         return self.fetch_json_data(
             "delete",
             "/v1/orgs/%s/owners" % orgname,
-            data={"username": username},
+            params={"username": username},
             x_with_authorization=True,
         )
 
     def create_team(self, orgname, teamname, description):
         return self.fetch_json_data(
             "post",
             "/v1/orgs/%s/teams" % orgname,
@@ -347,10 +343,10 @@
             x_with_authorization=True,
         )
 
     def remove_team_member(self, orgname, teamname, username):
         return self.fetch_json_data(
             "delete",
             "/v1/orgs/%s/teams/%s/members" % (orgname, teamname),
-            data={"username": username},
+            params={"username": username},
             x_with_authorization=True,
         )
```

### Comparing `platformio-6.1.6/platformio/account/commands/__init__.py` & `platformio-6.1.7/platformio/account/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/destroy.py` & `platformio-6.1.7/platformio/account/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/forgot.py` & `platformio-6.1.7/platformio/account/commands/forgot.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/login.py` & `platformio-6.1.7/platformio/account/commands/login.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/logout.py` & `platformio-6.1.7/platformio/account/commands/logout.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/password.py` & `platformio-6.1.7/platformio/account/commands/password.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/register.py` & `platformio-6.1.7/platformio/account/commands/register.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/show.py` & `platformio-6.1.7/platformio/account/commands/show.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/token.py` & `platformio-6.1.7/platformio/account/commands/token.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/commands/update.py` & `platformio-6.1.7/platformio/account/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/__init__.py` & `platformio-6.1.7/platformio/account/org/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/cli.py` & `platformio-6.1.7/platformio/account/org/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/__init__.py` & `platformio-6.1.7/platformio/account/org/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/add.py` & `platformio-6.1.7/platformio/account/org/commands/add.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/create.py` & `platformio-6.1.7/platformio/account/org/commands/create.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/destroy.py` & `platformio-6.1.7/platformio/account/org/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/list.py` & `platformio-6.1.7/platformio/account/org/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/remove.py` & `platformio-6.1.7/platformio/account/org/commands/remove.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/org/commands/update.py` & `platformio-6.1.7/platformio/account/team/commands/remove.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,42 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 
 from platformio.account.client import AccountClient
-from platformio.account.validate import validate_email, validate_orgname
+from platformio.account.validate import validate_orgname_teamname
 
 
-@click.command("update", short_help="Update organization")
-@click.argument("cur_orgname")
-@click.option(
-    "--orgname",
-    callback=lambda _, __, value: validate_orgname(value),
-    help="A new orgname",
+@click.command("remove", short_help="Remove a member from team")
+@click.argument(
+    "orgname_teamname",
+    metavar="ORGNAME:TEAMNAME",
+    callback=lambda _, __, value: validate_orgname_teamname(value),
 )
-@click.option("--email")
-@click.option("--displayname")
-def org_update_cmd(cur_orgname, **kwargs):
+@click.argument("username")
+def team_remove_cmd(orgname_teamname, username):
+    orgname, teamname = orgname_teamname.split(":", 1)
     client = AccountClient()
-    org = client.get_org(cur_orgname)
-    del org["owners"]
-    new_org = org.copy()
-    if not any(kwargs.values()):
-        for field in org:
-            new_org[field] = click.prompt(
-                field.replace("_", " ").capitalize(), default=org[field]
-            )
-            if field == "email":
-                validate_email(new_org[field])
-            if field == "orgname":
-                validate_orgname(new_org[field])
-    else:
-        new_org.update(
-            {key.replace("new_", ""): value for key, value in kwargs.items() if value}
-        )
-    client.update_org(cur_orgname, new_org)
+    client.remove_team_member(orgname, teamname, username)
     return click.secho(
-        "The organization `%s` has been successfully updated." % cur_orgname,
+        "The %s member has been successfully removed from the %s team."
+        % (username, teamname),
         fg="green",
     )
```

### Comparing `platformio-6.1.6/platformio/account/team/__init__.py` & `platformio-6.1.7/platformio/account/team/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/team/cli.py` & `platformio-6.1.7/platformio/account/team/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/team/commands/__init__.py` & `platformio-6.1.7/platformio/account/team/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/team/commands/add.py` & `platformio-6.1.7/platformio/account/team/commands/add.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/team/commands/create.py` & `platformio-6.1.7/platformio/account/team/commands/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,15 @@
 from platformio.account.validate import validate_orgname_teamname
 
 
 @click.command("create", short_help="Create a new team")
 @click.argument(
     "orgname_teamname",
     metavar="ORGNAME:TEAMNAME",
-    callback=lambda _, __, value: validate_orgname_teamname(
-        value, teamname_validate=True
-    ),
+    callback=lambda _, __, value: validate_orgname_teamname(value),
 )
 @click.option(
     "--description",
 )
 def team_create_cmd(orgname_teamname, description):
     orgname, teamname = orgname_teamname.split(":", 1)
     client = AccountClient()
```

### Comparing `platformio-6.1.6/platformio/account/team/commands/destroy.py` & `platformio-6.1.7/platformio/account/team/commands/destroy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/team/commands/list.py` & `platformio-6.1.7/platformio/account/team/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/account/team/commands/remove.py` & `platformio-6.1.7/platformio/registry/access/commands/revoke.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,27 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import click
 
-from platformio.account.client import AccountClient
-from platformio.account.validate import validate_orgname_teamname
+from platformio.registry.access.validate import validate_client, validate_urn
+from platformio.registry.client import RegistryClient
 
 
-@click.command("remove", short_help="Remove a member from team")
+@click.command("revoke", short_help="Revoke access")
 @click.argument(
-    "orgname_teamname",
-    metavar="ORGNAME:TEAMNAME",
-    callback=lambda _, __, value: validate_orgname_teamname(value),
+    "client",
+    metavar="[ORGNAME:TEAMNAME|USERNAME]",
+    callback=lambda _, __, value: validate_client(value),
 )
-@click.argument("username")
-def team_remove_cmd(orgname_teamname, username):
-    orgname, teamname = orgname_teamname.split(":", 1)
-    client = AccountClient()
-    client.remove_team_member(orgname, teamname, username)
+@click.argument(
+    "urn",
+    callback=lambda _, __, value: validate_urn(value),
+)
+@click.option("--urn-type", type=click.Choice(["prn:reg:pkg"]), default="prn:reg:pkg")
+def access_revoke_cmd(client, urn, urn_type):  # pylint: disable=unused-argument
+    reg_client = RegistryClient()
+    reg_client.revoke_access_from_resource(urn=urn, client=client)
     return click.secho(
-        "The %s member has been successfully removed from the %s team."
-        % (username, teamname),
+        "Access for resource %s has been revoked for %s" % (urn, client),
         fg="green",
     )
```

### Comparing `platformio-6.1.6/platformio/account/team/commands/update.py` & `platformio-6.1.7/platformio/account/team/commands/update.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,34 +22,30 @@
 @click.argument(
     "orgname_teamname",
     metavar="ORGNAME:TEAMNAME",
     callback=lambda _, __, value: validate_orgname_teamname(value),
 )
 @click.option(
     "--name",
-    callback=lambda _, __, value: validate_teamname(value),
+    callback=lambda _, __, value: validate_teamname(value) if value else value,
     help="A new team name",
 )
 @click.option(
     "--description",
 )
 def team_update_cmd(orgname_teamname, **kwargs):
     orgname, teamname = orgname_teamname.split(":", 1)
     client = AccountClient()
     team = client.get_team(orgname, teamname)
-    del team["id"]
-    del team["members"]
-    new_team = team.copy()
+    new_team = {
+        key: value if value is not None else team[key] for key, value in kwargs.items()
+    }
     if not any(kwargs.values()):
-        for field in team:
-            new_team[field] = click.prompt(
-                field.replace("_", " ").capitalize(), default=team[field]
-            )
-            if field == "name":
-                validate_teamname(new_team[field])
-    else:
-        new_team.update({key: value for key, value in kwargs.items() if value})
+        for key in kwargs:
+            new_team[key] = click.prompt(key.capitalize(), default=team[key])
+            if key == "name":
+                validate_teamname(new_team[key])
     client.update_team(orgname, teamname, new_team)
     return click.secho(
         "The team %s has been successfully updated." % teamname,
         fg="green",
     )
```

### Comparing `platformio-6.1.6/platformio/account/validate.py` & `platformio-6.1.7/platformio/account/validate.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,66 +14,71 @@
 
 import re
 
 import click
 
 
 def validate_username(value, field="username"):
-    value = str(value).strip()
-    if not re.match(r"^[a-z\d](?:[a-z\d]|-(?=[a-z\d])){0,37}$", value, flags=re.I):
+    value = str(value).strip() if value else None
+    if not value or not re.match(
+        r"^[a-z\d](?:[a-z\d]|-(?=[a-z\d])){0,37}$", value, flags=re.I
+    ):
         raise click.BadParameter(
             "Invalid %s format. "
             "%s must contain only alphanumeric characters "
             "or single hyphens, cannot begin or end with a hyphen, "
             "and must not be longer than 38 characters."
             % (field.lower(), field.capitalize())
         )
     return value
 
 
+def validate_orgname(value):
+    return validate_username(value, "Organization name")
+
+
 def validate_email(value):
-    value = str(value).strip()
-    if not re.match(r"^[a-z\d_\.\+\-]+@[a-z\d\-]+\.[a-z\d\-\.]+$", value, flags=re.I):
+    value = str(value).strip() if value else None
+    if not value or not re.match(
+        r"^[a-z\d_\.\+\-]+@[a-z\d\-]+\.[a-z\d\-\.]+$", value, flags=re.I
+    ):
         raise click.BadParameter("Invalid email address")
     return value
 
 
 def validate_password(value):
-    value = str(value).strip()
-    if not re.match(r"^(?=.*[a-z])(?=.*\d).{8,}$", value):
+    value = str(value).strip() if value else None
+    if not value or not re.match(r"^(?=.*[a-z])(?=.*\d).{8,}$", value):
         raise click.BadParameter(
             "Invalid password format. "
             "Password must contain at least 8 characters"
             " including a number and a lowercase letter"
         )
     return value
 
 
-def validate_orgname(value):
-    return validate_username(value, "Organization name")
-
-
-def validate_orgname_teamname(value, teamname_validate=False):
-    if ":" not in value:
-        raise click.BadParameter(
-            "Please specify organization and team name in the next"
-            " format - orgname:teamname. For example, mycompany:DreamTeam"
-        )
-    teamname = str(value.strip().split(":", 1)[1])
-    if teamname_validate:
-        validate_teamname(teamname)
-    return value
-
-
 def validate_teamname(value):
-    if not value:
-        return value
-    value = str(value).strip()
-    if not re.match(r"^[a-z\d](?:[a-z\d]|[\-_ ](?=[a-z\d])){0,19}$", value, flags=re.I):
+    value = str(value).strip() if value else None
+    if not value or not re.match(
+        r"^[a-z\d](?:[a-z\d]|[\-_ ](?=[a-z\d])){0,19}$", value, flags=re.I
+    ):
         raise click.BadParameter(
             "Invalid team name format. "
             "Team name must only contain alphanumeric characters, "
             "single hyphens, underscores, spaces. It can not "
             "begin or end with a hyphen or a underscore and must"
             " not be longer than 20 characters."
         )
     return value
+
+
+def validate_orgname_teamname(value):
+    value = str(value).strip() if value else None
+    if not value or ":" not in value:
+        raise click.BadParameter(
+            "Please specify organization and team name using the following"
+            " format - orgname:teamname. For example, mycompany:DreamTeam"
+        )
+    orgname, teamname = value.split(":", 1)
+    validate_orgname(orgname)
+    validate_teamname(teamname)
+    return value
```

### Comparing `platformio-6.1.6/platformio/app.py` & `platformio-6.1.7/platformio/app.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/system/99-platformio-udev.rules` & `platformio-6.1.7/platformio/assets/system/99-platformio-udev.rules`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/atom/.gcc-flags.json.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/atom/.gcc-flags.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/clion/CMakeLists.txt.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeLists.txt.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/clion/CMakeListsPrivate.txt.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/clion/CMakeListsPrivate.txt.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/codeblocks/platformio.cbp.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/codeblocks/platformio.cbp.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.cproject.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.cproject.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.project.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.project.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/sublimetext/platformio.sublime-project.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/sublimetext/platformio.sublime-project.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.filters.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.filters.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/visualstudio/platformio.vcxproj.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl` & `platformio-6.1.7/platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 %
 % def get_pio_configurations():
 %  predebug = {
 %    "type": "platformio-debug",
 %    "request": "launch",
 %    "name": "PIO Debug (skip Pre-Debug)",
 %    "executable": _escape_path(prog_path),
-%    "projectEnvName": env_name,
+%    "projectEnvName": env_name if forced_env_name else default_debug_env_name,
 %    "toolchainBinDir": _escape_path(os.path.dirname(gdb_path)),
 %    "internalConsoleOptions": "openOnSessionStart",
 %  }
 %
 %  if svd_path:
 %    predebug["svdPath"] = _escape_path(svd_path)
 %  end
 %  debug = predebug.copy()
 %  debug["name"] = "PIO Debug"
 %  debug["preLaunchTask"] = {
 %    "type": "PlatformIO",
-%    "task": ("Pre-Debug (%s)" % env_name) if len(config.envs()) > 1 and original_env_name else "Pre-Debug",
+%    "task": ("Pre-Debug (%s)" % env_name) if len(config.envs()) > 1 and forced_env_name else "Pre-Debug",
 %  }
 %  noloading = predebug.copy()
 %  noloading["name"] = "PIO Debug (without uploading)"
 %  noloading["loadMode"] = "manual"
 %  return [debug, predebug, noloading]
 % end
 %
```

### Comparing `platformio-6.1.6/platformio/builder/__init__.py` & `platformio-6.1.7/platformio/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/main.py` & `platformio-6.1.7/platformio/builder/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 from SCons.Script import AllowSubstExceptions  # pylint: disable=import-error
 from SCons.Script import AlwaysBuild  # pylint: disable=import-error
 from SCons.Script import Default  # pylint: disable=import-error
 from SCons.Script import DefaultEnvironment  # pylint: disable=import-error
 from SCons.Script import Import  # pylint: disable=import-error
 from SCons.Script import Variables  # pylint: disable=import-error
 
-from platformio import app, compat, fs
+from platformio import app, fs
 from platformio.platform.base import PlatformBase
-from platformio.proc import get_pythonexe_path
+from platformio.proc import get_pythonexe_path, where_is_program
 from platformio.project.helpers import get_project_dir
 
 AllowSubstExceptions(NameError)
 
 # append CLI arguments to build environment
 clivars = Variables(None)
 clivars.AddVariables(
@@ -95,14 +95,15 @@
     CXXCOM="Compiling",
 )
 if not int(ARGUMENTS.get("PIOVERBOSE", 0)):
     for name, value in command_strings.items():
         DEFAULT_ENV_OPTIONS["%sSTR" % name] = "%s $TARGET" % (value)
 
 env = DefaultEnvironment(**DEFAULT_ENV_OPTIONS)
+env.SConscriptChdir(False)
 
 # Load variables from CLI
 env.Replace(
     **{
         key: PlatformBase.decode_scons_arg(env[key])
         for key in list(clivars.keys())
         if key in env
@@ -135,27 +136,14 @@
     ],
 )
 
 if int(ARGUMENTS.get("ISATTY", 0)):
     # pylint: disable=protected-access
     click._compat.isatty = lambda stream: True
 
-if compat.IS_WINDOWS and sys.version_info >= (3, 8) and os.getcwd().startswith("\\\\"):
-    click.secho("!!! WARNING !!!\t\t" * 3, fg="red")
-    click.secho(
-        "Your project is located on a mapped network drive but the "
-        "current command-line shell does not support the UNC paths.",
-        fg="yellow",
-    )
-    click.secho(
-        "Please move your project to a physical drive or check this workaround: "
-        "https://bit.ly/3kuU5mP\n",
-        fg="yellow",
-    )
-
 if env.subst("$BUILD_CACHE_DIR"):
     if not os.path.isdir(env.subst("$BUILD_CACHE_DIR")):
         os.makedirs(env.subst("$BUILD_CACHE_DIR"))
     env.CacheDir("$BUILD_CACHE_DIR")
 
 if not int(ARGUMENTS.get("PIOVERBOSE", 0)):
     click.echo("Verbose mode can be enabled via `-v, --verbose` option")
@@ -166,37 +154,35 @@
 
 if not os.path.isdir(env.subst("$BUILD_DIR")):
     os.makedirs(env.subst("$BUILD_DIR"))
 
 env.LoadProjectOptions()
 env.LoadPioPlatform()
 
-env.SConscriptChdir(0)
 env.SConsignFile(
     os.path.join(
-        "$BUILD_DIR", ".sconsign%d%d" % (sys.version_info[0], sys.version_info[1])
+        "$BUILD_CACHE_DIR" if env.subst("$BUILD_CACHE_DIR") else "$BUILD_DIR",
+        ".sconsign%d%d" % (sys.version_info[0], sys.version_info[1]),
     )
 )
 
-for item in env.GetExtraScripts("pre"):
-    env.SConscript(item, exports="env")
+env.SConscript(env.GetExtraScripts("pre"), exports="env")
 
 if env.IsCleanTarget():
-    env.CleanProject("cleanall" in COMMAND_LINE_TARGETS)
+    env.CleanProject(fullclean=int(ARGUMENTS.get("FULLCLEAN", 0)))
     env.Exit(0)
 
 env.SConscript("$BUILD_SCRIPT")
 
 if "UPLOAD_FLAGS" in env:
     env.Prepend(UPLOADERFLAGS=["$UPLOAD_FLAGS"])
 if env.GetProjectOption("upload_command"):
     env.Replace(UPLOADCMD=env.GetProjectOption("upload_command"))
 
-for item in env.GetExtraScripts("post"):
-    env.SConscript(item, exports="env")
+env.SConscript(env.GetExtraScripts("post"), exports="env")
 
 ##############################################################################
 
 # Checking program size
 if env.get("SIZETOOL") and not (
     set(["nobuild", "sizedata"]) & set(COMMAND_LINE_TARGETS)
 ):
@@ -204,14 +190,21 @@
     # Replace platform's "size" target with our
     _new_targets = [t for t in DEFAULT_TARGETS if str(t) != "size"]
     Default(None)
     Default(_new_targets)
     Default("checkprogsize")
 
 if "compiledb" in COMMAND_LINE_TARGETS:
+    # Resolve absolute path of toolchain
+    for cmd in ("CC", "CXX", "AS"):
+        if cmd not in env:
+            continue
+        if os.path.isabs(env[cmd]):
+            continue
+        env[cmd] = where_is_program(env.subst("$%s" % cmd), env.subst("${ENV['PATH']}"))
     env.Alias("compiledb", env.CompilationDatabase("$COMPILATIONDB_PATH"))
 
 # Print configured protocols
 env.AddPreAction(
     "upload",
     env.VerboseAction(
         lambda source, target, env: env.PrintUploadInfo(),
@@ -253,7 +246,13 @@
             "sizedata",
             DEFAULT_TARGETS,
             env.VerboseAction(env.DumpSizeData, "Generating memory usage report..."),
         )
     )
 
     Default("sizedata")
+
+# issue #4604: process targets sequentially
+for index, target in enumerate(
+    [t for t in COMMAND_LINE_TARGETS if not t.startswith("__")][1:]
+):
+    env.Depends(target, COMMAND_LINE_TARGETS[index])
```

### Comparing `platformio-6.1.6/platformio/builder/tools/__init__.py` & `platformio-6.1.7/platformio/builder/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/pioasm.py` & `platformio-6.1.7/platformio/builder/tools/pioasm.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/piobuild.py` & `platformio-6.1.7/platformio/builder/tools/piobuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,15 @@
     if not flags:
         return
     parsed = env.ParseFlagsExtended(flags)
     unflag_scopes = tuple(set(["ASPPFLAGS"] + list(parsed.keys())))
     for scope in unflag_scopes:
         for unflags in parsed.values():
             for unflag in unflags:
-                for current in env.get(scope, []):
+                for current in list(env.get(scope, [])):
                     conditions = [
                         unflag == current,
                         not isinstance(unflag, (tuple, list))
                         and isinstance(current, (tuple, list))
                         and unflag == current[0],
                     ]
                     if any(conditions):
```

### Comparing `platformio-6.1.6/platformio/builder/tools/piohooks.py` & `platformio-6.1.7/platformio/builder/tools/piohooks.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/pioino.py` & `platformio-6.1.7/platformio/builder/tools/pioino.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import click
 
 from platformio.compat import get_filesystem_encoding, get_locale_encoding
 
 
 class InoToCPPConverter:
-
     PROTOTYPE_RE = re.compile(
         r"""^(
         (?:template\<.*\>\s*)?      # template
         ([a-z_\d\&]+\*?\s+){1,2}    # return type
         ([a-z_\d]+\s*)              # name of prototype
         \([a-z_,\.\*\&\[\]\s\d]*\)  # arguments
         )\s*(\{|;)                  # must end with `{` or `;`
@@ -99,15 +98,15 @@
 
         if not self._main_ino:
             self._main_ino = nodes[0].get_path()
 
         return "\n".join(["#include <Arduino.h>"] + lines) if lines else None
 
     def process(self, contents):
-        out_file = self._main_ino + ".cpp"
+        out_file = re.sub(r"[\"\'\;]+", "", self._main_ino) + ".cpp"
         assert self._gcc_preprocess(contents, out_file)
         contents = self.read_safe_contents(out_file)
         contents = self._join_multiline_strings(contents)
         self.write_safe_contents(out_file, self.append_prototypes(contents))
         return out_file
 
     def _gcc_preprocess(self, contents, out_file):
```

### Comparing `platformio-6.1.6/platformio/builder/tools/piointegration.py` & `platformio-6.1.7/platformio/builder/tools/piointegration.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/piolib.py` & `platformio-6.1.7/platformio/builder/tools/piolib.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import SCons.Scanner  # pylint: disable=import-error
 from SCons.Script import ARGUMENTS  # pylint: disable=import-error
 from SCons.Script import DefaultEnvironment  # pylint: disable=import-error
 
 from platformio import exception, fs
 from platformio.builder.tools import piobuild
 from platformio.compat import IS_WINDOWS, hashlib_encode_data, string_types
-from platformio.http import HTTPClientError, InternetIsOffline
+from platformio.http import HTTPClientError, InternetConnectionError
 from platformio.package.exception import (
     MissingPackageManifestError,
     UnknownPackageError,
 )
 from platformio.package.manager.library import LibraryPackageManager
 from platformio.package.manifest.parser import (
     ManifestParserError,
@@ -105,15 +105,14 @@
                     return ["arduino"]
                 if "mbed.h" in content and include_re.search(content):
                     return ["mbed"]
         return []
 
 
 class LibBuilderBase:
-
     CLASSIC_SCANNER = SCons.Scanner.C.CScanner()
     CCONDITIONAL_SCANNER = SCons.Scanner.C.CConditionalScanner()
     # Max depth of nested includes:
     # -1 = unlimited
     # 0 - disabled nesting
     # >0 - number of allowed nested includes
     CCONDITIONAL_SCANNER_DEPTH = 99
@@ -294,19 +293,20 @@
     def load_manifest(self):
         return {}
 
     def process_extra_options(self):
         with fs.cd(self.path):
             self.env.ProcessFlags(self.build_flags)
             if self.extra_script:
-                self.env.SConscriptChdir(1)
+                self.env.SConscriptChdir(True)
                 self.env.SConscript(
                     os.path.abspath(self.extra_script),
                     exports={"env": self.env, "pio_lib_builder": self},
                 )
+                self.env.SConscriptChdir(False)
             self.env.ProcessUnFlags(self.build_unflags)
 
     def process_dependencies(self):
         if not self.dependencies or self._deps_are_processed:
             return
         self._deps_are_processed = True
         for item in self.dependencies:
@@ -978,15 +978,19 @@
         lm = LibraryPackageManager(
             self.env.subst(os.path.join("$PROJECT_LIBDEPS_DIR", "$PIOENV"))
         )
         for spec in not_found_specs:
             try:
                 lm.install(spec)
                 did_install = True
-            except (HTTPClientError, UnknownPackageError, InternetIsOffline) as exc:
+            except (
+                HTTPClientError,
+                UnknownPackageError,
+                InternetConnectionError,
+            ) as exc:
                 click.secho("Warning! %s" % exc, fg="yellow")
 
         # reset cache
         if did_install:
             DefaultEnvironment().Replace(__PIO_LIB_BUILDERS=None)
 
     def process_dependencies(self):  # pylint: disable=too-many-branches
@@ -1153,15 +1157,15 @@
                     " (License: %s, " % (_get_lib_license(pkg) or "Unknown"), nl=False
                 )
                 if pkg.metadata and pkg.metadata.spec.external:
                     click.echo("URI: %s, " % pkg.metadata.spec.uri, nl=False)
                 click.echo("Path: %s" % lb.path, nl=False)
                 click.echo(")", nl=False)
             click.echo("")
-            if lb.depbuilders:
+            if lb.verbose and lb.depbuilders:
                 _print_deps_tree(lb, level + 1)
 
     project = ProjectAsLibBuilder(env, "$PROJECT_DIR")
 
     if "test" in env["BUILD_TYPE"]:
         project.env.ConfigureTestTarget()
```

### Comparing `platformio-6.1.6/platformio/builder/tools/piomaxlen.py` & `platformio-6.1.7/platformio/builder/tools/piomaxlen.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/piomisc.py` & `platformio-6.1.7/platformio/builder/tools/piomisc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/pioplatform.py` & `platformio-6.1.7/platformio/builder/tools/pioplatform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/pioproject.py` & `platformio-6.1.7/platformio/builder/tools/pioproject.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/piosize.py` & `platformio-6.1.7/platformio/builder/tools/piosize.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/piotarget.py` & `platformio-6.1.7/platformio/builder/tools/piotarget.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,31 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from SCons.Action import Action  # pylint: disable=import-error
 from SCons.Script import ARGUMENTS  # pylint: disable=import-error
-from SCons.Script import COMMAND_LINE_TARGETS  # pylint: disable=import-error
 from SCons.Script import AlwaysBuild  # pylint: disable=import-error
 
 from platformio import compat, fs
 
 
 def VerboseAction(_, act, actstr):
     if int(ARGUMENTS.get("PIOVERBOSE", 0)):
         return act
     return Action(act, actstr)
 
 
 def IsCleanTarget(env):
-    return env.GetOption("clean") or ("cleanall" in COMMAND_LINE_TARGETS)
+    return env.GetOption("clean")
 
 
-def CleanProject(env, clean_all=False):
+def CleanProject(env, fullclean=False):
     def _relpath(path):
         if compat.IS_WINDOWS:
             prefix = os.getcwd()[:2].lower()
             if (
                 ":" not in prefix
                 or not path.lower().startswith(prefix)
                 or os.path.relpath(path).startswith("..")
@@ -52,15 +51,15 @@
     build_dir = env.subst("$BUILD_DIR")
     libdeps_dir = env.subst(os.path.join("$PROJECT_LIBDEPS_DIR", "$PIOENV"))
     if os.path.isdir(build_dir):
         _clean_dir(build_dir)
     else:
         print("Build environment is clean")
 
-    if clean_all and os.path.isdir(libdeps_dir):
+    if fullclean and os.path.isdir(libdeps_dir):
         _clean_dir(libdeps_dir)
 
     print("Done cleaning")
 
 
 def AddTarget(  # pylint: disable=too-many-arguments
     env,
```

### Comparing `platformio-6.1.6/platformio/builder/tools/piotest.py` & `platformio-6.1.7/platformio/builder/tools/piotest.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/builder/tools/pioupload.py` & `platformio-6.1.7/platformio/builder/tools/pioupload.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/cache.py` & `platformio-6.1.7/platformio/cache.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/check/__init__.py` & `platformio-6.1.7/platformio/check/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/check/cli.py` & `platformio-6.1.7/platformio/check/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,26 +34,23 @@
 
 @click.command("check", short_help="Static Code Analysis")
 @click.option("-e", "--environment", multiple=True)
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=True, writable=True),
 )
 @click.option(
     "-c",
     "--project-conf",
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
 )
-@click.option("--pattern", multiple=True)
+@click.option("--pattern", multiple=True, hidden=True)
+@click.option("-f", "--src-filters", multiple=True)
 @click.option("--flags", multiple=True)
 @click.option(
     "--severity", multiple=True, type=click.Choice(DefectItem.SEVERITY_LABELS.values())
 )
 @click.option("-s", "--silent", is_flag=True)
 @click.option("-v", "--verbose", is_flag=True)
 @click.option("--json-output", is_flag=True)
@@ -63,14 +60,15 @@
     type=click.Choice(DefectItem.SEVERITY_LABELS.values()),
 )
 @click.option("--skip-packages", is_flag=True)
 def cli(
     environment,
     project_dir,
     project_conf,
+    src_filters,
     pattern,
     flags,
     severity,
     silent,
     verbose,
     json_output,
     fail_on_defect,
@@ -101,22 +99,32 @@
             for k, v in env_options.items():
                 if k not in ("platform", "framework", "board"):
                     continue
                 env_dump.append(
                     "%s: %s" % (k, ", ".join(v) if isinstance(v, list) else v)
                 )
 
-            default_patterns = [
-                config.get("platformio", "src_dir"),
-                config.get("platformio", "include_dir"),
+            default_src_filters = [
+                "+<%s>" % os.path.basename(config.get("platformio", "src_dir")),
+                "+<%s>" % os.path.basename(config.get("platformio", "include_dir")),
             ]
+
+            src_filters = (
+                src_filters
+                or pattern
+                or env_options.get(
+                    "check_src_filters",
+                    env_options.get("check_patterns", default_src_filters),
+                )
+            )
+
             tool_options = dict(
                 verbose=verbose,
                 silent=silent,
-                patterns=pattern or env_options.get("check_patterns", default_patterns),
+                src_filters=src_filters,
                 flags=flags or env_options.get("check_flags"),
                 severity=[DefectItem.SEVERITY_LABELS[DefectItem.SEVERITY_HIGH]]
                 if silent
                 else severity or config.get("env:" + envname, "check_severity"),
                 skip_packages=skip_packages or env_options.get("check_skip_packages"),
                 platform_packages=env_options.get("platform_packages"),
             )
@@ -261,15 +269,15 @@
 
     total = ["Total"] + [sum(d) for d in list(zip(*tabular_data))[1:]]
     tabular_data.sort()
     tabular_data.append([])  # Empty line as delimiter
     tabular_data.append(total)
 
     headers = ["Component"]
-    headers.extend([l.upper() for l in severity_labels])
+    headers.extend([label.upper() for label in severity_labels])
     headers = [click.style(h, bold=True) for h in headers]
     click.echo(tabulate(tabular_data, headers=headers, numalign="center"))
     click.echo()
 
 
 def print_check_summary(results, verbose=False):
     click.echo()
```

### Comparing `platformio-6.1.6/platformio/check/defect.py` & `platformio-6.1.7/platformio/check/defect.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 import click
 
+from platformio.exception import PlatformioException
 from platformio.project.helpers import get_project_dir
 
 # pylint: disable=too-many-instance-attributes, redefined-builtin
 # pylint: disable=too-many-arguments
 
 
 class DefectItem:
-
     SEVERITY_HIGH = 1
     SEVERITY_MEDIUM = 2
     SEVERITY_LOW = 4
     SEVERITY_LABELS = {4: "low", 2: "medium", 1: "high"}
 
     def __init__(
         self,
@@ -75,15 +75,15 @@
         return self.severity | defect.severity
 
     @staticmethod
     def severity_to_int(label):
         for key, value in DefectItem.SEVERITY_LABELS.items():
             if label == value:
                 return key
-        raise Exception("Unknown severity label -> %s" % label)
+        raise PlatformioException("Unknown severity label -> %s" % label)
 
     def as_dict(self):
         return {
             "severity": self.SEVERITY_LABELS[self.severity],
             "category": self.category,
             "message": self.message,
             "file": os.path.abspath(self.file),
```

### Comparing `platformio-6.1.6/platformio/check/tools/__init__.py` & `platformio-6.1.7/platformio/check/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/check/tools/base.py` & `platformio-6.1.7/platformio/check/tools/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import glob
 import os
 import tempfile
 
 import click
 
 from platformio import fs, proc
 from platformio.check.defect import DefectItem
@@ -26,42 +25,43 @@
 
 
 class CheckToolBase:  # pylint: disable=too-many-instance-attributes
     def __init__(self, project_dir, config, envname, options):
         self.config = config
         self.envname = envname
         self.options = options
+        self.project_dir = project_dir
         self.cc_flags = []
         self.cxx_flags = []
         self.cpp_includes = []
         self.cpp_defines = []
         self.toolchain_defines = []
         self._tmp_files = []
         self.cc_path = None
         self.cxx_path = None
         self._defects = []
         self._on_defect_callback = None
         self._bad_input = False
-        self._load_cpp_data(project_dir)
+        self._load_cpp_data()
 
         # detect all defects by default
         if not self.options.get("severity"):
             self.options["severity"] = [
                 DefectItem.SEVERITY_LOW,
                 DefectItem.SEVERITY_MEDIUM,
                 DefectItem.SEVERITY_HIGH,
             ]
         # cast to severity by ids
         self.options["severity"] = [
             s if isinstance(s, int) else DefectItem.severity_to_int(s)
             for s in self.options["severity"]
         ]
 
-    def _load_cpp_data(self, project_dir):
-        data = load_build_metadata(project_dir, self.envname)
+    def _load_cpp_data(self):
+        data = load_build_metadata(self.project_dir, self.envname)
         if not data:
             return
         self.cc_flags = click.parser.split_arg_string(data.get("cc_flags", ""))
         self.cxx_flags = click.parser.split_arg_string(data.get("cxx_flags", ""))
         self.cpp_includes = self._dump_includes(data.get("includes", {}))
         self.cpp_defines = data.get("defines", [])
         self.cc_path = data.get("cc_path")
@@ -95,14 +95,21 @@
                 language,
                 " ".join(
                     [f for f in build_flags if f.startswith(("-m", "-f", "-std"))]
                 ),
                 includes_file,
             )
             result = proc.exec_command(cmd, shell=True)
+
+            if result["returncode"] != 0:
+                click.echo("Warning: Failed to extract toolchain defines!")
+                if self.options.get("verbose"):
+                    click.echo(result["out"])
+                    click.echo(result["err"])
+
             for line in result["out"].split("\n"):
                 tokens = line.strip().split(" ", 2)
                 if not tokens or tokens[0] != "#define":
                     continue
                 if len(tokens) > 2:
                     defines.append("%s=%s" % (tokens[1], tokens[2]))
                 else:
@@ -197,36 +204,32 @@
                 click.echo(result["out"])
                 click.echo(result["err"])
             self._bad_input = True
 
         return result
 
     @staticmethod
-    def get_project_target_files(patterns):
+    def get_project_target_files(project_dir, src_filters):
         c_extension = (".c",)
         cpp_extensions = (".cc", ".cpp", ".cxx", ".ino")
         header_extensions = (".h", ".hh", ".hpp", ".hxx")
 
         result = {"c": [], "c++": [], "headers": []}
 
         def _add_file(path):
             if path.endswith(header_extensions):
                 result["headers"].append(os.path.abspath(path))
             elif path.endswith(c_extension):
                 result["c"].append(os.path.abspath(path))
             elif path.endswith(cpp_extensions):
                 result["c++"].append(os.path.abspath(path))
 
-        for pattern in patterns:
-            for item in glob.glob(pattern, recursive=True):
-                if not os.path.isdir(item):
-                    _add_file(item)
-                for root, _, files in os.walk(item, followlinks=True):
-                    for f in files:
-                        _add_file(os.path.join(root, f))
+        src_filters = normalize_src_filters(src_filters)
+        for f in fs.match_src_files(project_dir, src_filters):
+            _add_file(f)
 
         return result
 
     def check(self, on_defect_callback=None):
         self._on_defect_callback = on_defect_callback
         cmd = self.configure_command()
         if cmd:
@@ -239,7 +242,26 @@
             if self.options.get("verbose"):
                 click.echo("Error: Couldn't configure command")
             self._bad_input = True
 
         self.clean_up()
 
         return self._bad_input
+
+
+#
+# Helpers
+#
+
+
+def normalize_src_filters(src_filters):
+    def _normalize(src_filters):
+        return (
+            src_filters
+            if src_filters.startswith(("+<", "-<"))
+            else "+<%s>" % src_filters
+        )
+
+    if isinstance(src_filters, (list, tuple)):
+        return " ".join([_normalize(f) for f in src_filters])
+
+    return _normalize(src_filters)
```

### Comparing `platformio-6.1.6/platformio/check/tools/clangtidy.py` & `platformio-6.1.7/platformio/check/tools/clangtidy.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         cmd = [tool_path, "--quiet"]
         flags = self.get_flags("clangtidy")
         if not (
             self.is_flag_set("--checks", flags) or self.is_flag_set("--config", flags)
         ):
             cmd.append("--checks=*")
 
-        project_files = self.get_project_target_files(self.options["patterns"])
+        project_files = self.get_project_target_files(
+            self.project_dir, self.options["src_filters"]
+        )
 
         src_files = []
         for items in project_files.values():
             src_files.extend(items)
 
         cmd.extend(flags + src_files + ["--"])
         cmd.extend(
```

### Comparing `platformio-6.1.6/platformio/check/tools/cppcheck.py` & `platformio-6.1.7/platformio/check/tools/cppcheck.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                         "Error: Found a breaking defect '%s' in %s:%s\n"
                         "Please note: check results might not be valid!\n"
                         "Try adding --skip-packages"
                         % (args.get("message"), args.get("file"), args.get("line"))
                     )
                     click.echo()
                 self._bad_input = True
-                self._buffer = ""
+            self._buffer = ""
             return None
 
         self._buffer = ""
         return DefectItem(**args)
 
     def configure_command(self, language, src_file):  # pylint: disable=arguments-differ
         tool_path = os.path.join(self.get_tool_dir("tool-cppcheck"), "cppcheck")
@@ -210,15 +210,17 @@
     def clean_up(self):
         super().clean_up()
 
         # delete temporary dump files generated by addons
         if not self.is_flag_set("--addon", self.get_flags("cppcheck")):
             return
 
-        for files in self.get_project_target_files(self.options["patterns"]).values():
+        for files in self.get_project_target_files(
+            self.project_dir, self.options["src_filters"]
+        ).values():
             for f in files:
                 dump_file = f + ".dump"
                 if os.path.isfile(dump_file):
                     os.remove(dump_file)
 
     @staticmethod
     def is_check_successful(cmd_result):
@@ -239,15 +241,17 @@
         return flag.replace("gnu", "c").replace(
             standard, cpp_standards_map.get(standard, standard)
         )
 
     def check(self, on_defect_callback=None):
         self._on_defect_callback = on_defect_callback
 
-        project_files = self.get_project_target_files(self.options["patterns"])
+        project_files = self.get_project_target_files(
+            self.project_dir, self.options["src_filters"]
+        )
         src_files_scope = ("c", "c++")
         if not any(project_files[t] for t in src_files_scope):
             click.echo("Error: Nothing to check.")
             return True
 
         for scope, files in project_files.items():
             if scope not in src_files_scope:
```

### Comparing `platformio-6.1.6/platformio/check/tools/pvsstudio.py` & `platformio-6.1.7/platformio/check/tools/pvsstudio.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         return (
             "license" not in cmd_result["err"].lower() and cmd_result["returncode"] == 0
         )
 
     def check(self, on_defect_callback=None):
         self._on_defect_callback = on_defect_callback
         for scope, files in self.get_project_target_files(
-            self.options["patterns"]
+            self.project_dir, self.options["src_filters"]
         ).items():
             if scope not in ("c", "c++"):
                 continue
             for src_file in files:
                 self._prepare_preprocessed_file(src_file)
                 cmd = self.configure_command(src_file)
                 if self.options.get("verbose"):
```

### Comparing `platformio-6.1.6/platformio/cli.py` & `platformio-6.1.7/platformio/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 import importlib
 from pathlib import Path
 
 import click
 
 
 class PlatformioCLI(click.MultiCommand):
-
     leftover_args = []
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._pio_root_path = Path(__file__).parent
         self._pio_cmd_aliases = dict(package="pkg")
```

### Comparing `platformio-6.1.6/platformio/commands/__init__.py` & `platformio-6.1.7/platformio/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/commands/boards.py` & `platformio-6.1.7/platformio/commands/boards.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         ):
             continue
         if board["platform"] not in grpboards:
             grpboards[board["platform"]] = []
         grpboards[board["platform"]].append(board)
 
     terminal_width = shutil.get_terminal_size().columns
-    for (platform, boards) in sorted(grpboards.items()):
+    for platform, boards in sorted(grpboards.items()):
         click.echo("")
         click.echo("Platform: ", nl=False)
         click.secho(platform, bold=True)
         click.echo("=" * terminal_width)
         print_boards(boards)
     return True
```

### Comparing `platformio-6.1.6/platformio/commands/ci.py` & `platformio-6.1.7/platformio/commands/ci.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,23 +47,21 @@
 @click.argument("src", nargs=-1, callback=validate_path)
 @click.option("-l", "--lib", multiple=True, callback=validate_path, metavar="DIRECTORY")
 @click.option("--exclude", multiple=True)
 @click.option("-b", "--board", multiple=True, metavar="ID", callback=validate_boards)
 @click.option(
     "--build-dir",
     default=tempfile.mkdtemp,
-    type=click.Path(file_okay=False, dir_okay=True, writable=True, resolve_path=True),
+    type=click.Path(file_okay=False, dir_okay=True, writable=True),
 )
 @click.option("--keep-build-dir", is_flag=True)
 @click.option(
     "-c",
     "--project-conf",
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
 )
 @click.option("-O", "--project-option", multiple=True)
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("-v", "--verbose", is_flag=True)
 @click.pass_context
 def cli(  # pylint: disable=too-many-arguments, too-many-branches
     ctx,
@@ -105,16 +103,16 @@
         if exclude:
             _exclude_contents(build_dir, exclude)
 
         # initialise project
         ctx.invoke(
             project_init_cmd,
             project_dir=build_dir,
-            board=board,
-            project_option=project_option,
+            boards=board,
+            project_options=project_option,
         )
 
         # process project
         ctx.invoke(
             cmd_run, project_dir=build_dir, environment=environments, verbose=verbose
         )
     finally:
```

### Comparing `platformio-6.1.6/platformio/commands/device/__init__.py` & `platformio-6.1.7/platformio/commands/device/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/commands/lib.py` & `platformio-6.1.7/platformio/commands/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,17 +61,15 @@
 
 @click.group(short_help="Library manager", hidden=True)
 @click.option(
     "-d",
     "--storage-dir",
     multiple=True,
     default=None,
-    type=click.Path(
-        exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
     help="Manage custom library storage",
 )
 @click.option(
     "-g", "--global", is_flag=True, help="Manage global PlatformIO library storage"
 )
 @click.option(
     "-e",
```

### Comparing `platformio-6.1.6/platformio/commands/platform.py` & `platformio-6.1.7/platformio/commands/platform.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/commands/settings.py` & `platformio-6.1.7/platformio/commands/settings.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/commands/update.py` & `platformio-6.1.7/platformio/commands/update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/commands/upgrade.py` & `platformio-6.1.7/platformio/commands/upgrade.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,118 +9,92 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
-import os
 import re
-from zipfile import ZipFile
+import subprocess
 
 import click
 
 from platformio import VERSION, __version__, app, exception
-from platformio.compat import IS_WINDOWS
 from platformio.http import fetch_remote_content
 from platformio.package.manager.core import update_core_packages
-from platformio.proc import exec_command, get_pythonexe_path
-from platformio.project.helpers import get_project_cache_dir
+from platformio.proc import get_pythonexe_path
+
+PYPI_JSON_URL = "https://pypi.org/pypi/platformio/json"
+DEVELOP_ZIP_URL = "https://github.com/platformio/platformio-core/archive/develop.zip"
+DEVELOP_INIT_SCRIPT_URL = (
+    "https://raw.githubusercontent.com/platformio/platformio-core"
+    "/develop/platformio/__init__.py"
+)
 
 
 @click.command("upgrade", short_help="Upgrade PlatformIO Core to the latest version")
 @click.option("--dev", is_flag=True, help="Use development branch")
-def cli(dev):
+@click.option("--verbose", "-v", is_flag=True)
+def cli(dev, verbose):
     update_core_packages()
     if not dev and __version__ == get_latest_version():
         return click.secho(
             "You're up-to-date!\nPlatformIO %s is currently the "
             "newest version available." % __version__,
             fg="green",
         )
 
-    click.secho("Please wait while upgrading PlatformIO ...", fg="yellow")
+    click.secho("Please wait while upgrading PlatformIO Core ...", fg="yellow")
 
+    python_exe = get_pythonexe_path()
     to_develop = dev or not all(c.isdigit() for c in __version__ if c != ".")
-    cmds = (
-        ["pip", "install", "--upgrade", download_dist_package(to_develop)],
-        ["platformio", "--version"],
-    )
+    pkg_spec = DEVELOP_ZIP_URL if to_develop else "platformio"
 
-    cmd = None
-    r = {}
     try:
-        for cmd in cmds:
-            cmd = [get_pythonexe_path(), "-m"] + cmd
-            r = exec_command(cmd)
-
-            # try pip with disabled cache
-            if r["returncode"] != 0 and cmd[2] == "pip":
-                cmd.insert(3, "--no-cache-dir")
-                r = exec_command(cmd)
-
-            assert r["returncode"] == 0
-        assert "version" in r["out"]
-        actual_version = r["out"].strip().split("version", 1)[1].strip()
+        subprocess.run(
+            [python_exe, "-m", "pip", "install", "--upgrade", pkg_spec],
+            check=True,
+            capture_output=not verbose,
+        )
+        r = subprocess.run(
+            [python_exe, "-m", "platformio", "--version"],
+            check=True,
+            capture_output=True,
+            text=True,
+        )
+        assert "version" in r.stdout
+        actual_version = r.stdout.split("version", 1)[1].strip()
         click.secho(
             "PlatformIO has been successfully upgraded to %s" % actual_version,
             fg="green",
         )
         click.echo("Release notes: ", nl=False)
         click.secho("https://docs.platformio.org/en/latest/history.html", fg="cyan")
         if app.get_session_var("caller_id"):
             click.secho(
                 "Warning! Please restart IDE to affect PIO Home changes", fg="yellow"
             )
-    except Exception as exc:
-        if not r:
-            raise exception.UpgradeError("\n".join([str(cmd), str(exc)])) from exc
-        permission_errors = ("permission denied", "not permitted")
-        if any(m in r["err"].lower() for m in permission_errors) and not IS_WINDOWS:
-            click.secho(
-                """
------------------
-Permission denied
------------------
-You need the `sudo` permission to install Python packages. Try
-
-> sudo pip install -U platformio
-
-WARNING! Don't use `sudo` for the rest PlatformIO commands.
-""",
-                fg="yellow",
-                err=True,
-            )
-            raise exception.ReturnErrorCode(1)
-        raise exception.UpgradeError("\n".join([str(cmd), r["out"], r["err"]]))
+    except (AssertionError, subprocess.CalledProcessError) as exc:
+        click.secho(
+            "\nWarning!!! Could not automatically upgrade the PlatformIO Core.",
+            fg="red",
+        )
+        click.secho(
+            "Please upgrade it manually using the following command:\n",
+            fg="red",
+        )
+        click.secho(f'"{python_exe}" -m pip install -U {pkg_spec}\n', fg="cyan")
+        raise exception.ReturnErrorCode(1) from exc
 
     return True
 
 
-def download_dist_package(to_develop):
-    if not to_develop:
-        return "platformio"
-    dl_url = "https://github.com/platformio/platformio-core/archive/develop.zip"
-    cache_dir = get_project_cache_dir()
-    if not os.path.isdir(cache_dir):
-        os.makedirs(cache_dir)
-    pkg_name = os.path.join(cache_dir, "piocoredevelop.zip")
-    try:
-        with open(pkg_name, "wb") as fp:
-            r = exec_command(
-                ["curl", "-fsSL", dl_url], stdout=fp, universal_newlines=True
-            )
-            assert r["returncode"] == 0
-        # check ZIP structure
-        with ZipFile(pkg_name) as zp:
-            assert zp.testzip() is None
-        return pkg_name
-    except:  # pylint: disable=bare-except
-        pass
-    return dl_url
+def get_pkg_spec(to_develop):
+    if to_develop:
+        return
 
 
 def get_latest_version():
     try:
         if not str(VERSION[2]).isdigit():
             try:
                 return get_develop_latest_version()
@@ -129,18 +103,15 @@
         return get_pypi_latest_version()
     except Exception as exc:
         raise exception.GetLatestVersionError() from exc
 
 
 def get_develop_latest_version():
     version = None
-    content = fetch_remote_content(
-        "https://raw.githubusercontent.com/platformio/platformio"
-        "/develop/platformio/__init__.py"
-    )
+    content = fetch_remote_content(DEVELOP_INIT_SCRIPT_URL)
     for line in content.split("\n"):
         line = line.strip()
         if not line.startswith("VERSION"):
             continue
         match = re.match(r"VERSION\s*=\s*\(([^\)]+)\)", line)
         if not match:
             continue
@@ -149,9 +120,9 @@
             version = version.replace(c, "")
         version = ".".join(version.split(","))
     assert version
     return version
 
 
 def get_pypi_latest_version():
-    content = fetch_remote_content("https://pypi.org/pypi/platformio/json")
+    content = fetch_remote_content(PYPI_JSON_URL)
     return json.loads(content)["info"]["version"]
```

### Comparing `platformio-6.1.6/platformio/compat.py` & `platformio-6.1.7/platformio/compat.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/debug/__init__.py` & `platformio-6.1.7/platformio/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/debug/cli.py` & `platformio-6.1.7/platformio/debug/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,40 +24,36 @@
 
 from platformio import app, exception, fs, proc
 from platformio.compat import IS_WINDOWS
 from platformio.debug import helpers
 from platformio.debug.config.factory import DebugConfigFactory
 from platformio.debug.exception import DebugInvalidOptionsError
 from platformio.debug.process.gdb import GDBClientProcess
+from platformio.exception import ReturnErrorCode
 from platformio.platform.factory import PlatformFactory
 from platformio.project.config import ProjectConfig
-from platformio.project.exception import ProjectEnvsNotAvailableError
 from platformio.project.helpers import is_platformio_project
 from platformio.project.options import ProjectOptions
 
 
 @click.command(
     "debug",
     context_settings=dict(ignore_unknown_options=True),
     short_help="Unified Debugger",
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
 )
 @click.option(
     "-c",
     "--project-conf",
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
 )
 @click.option("--environment", "-e", metavar="<environment>")
 @click.option("--load-mode", type=ProjectOptions["env.debug_load_mode"].type)
 @click.option("--verbose", "-v", is_flag=True)
 @click.option("--interface", type=click.Choice(["gdb"]))
 @click.argument("__unprocessed", nargs=-1, type=click.UNPROCESSED)
 @click.pass_context
@@ -77,69 +73,65 @@
     for name in ("CWD", "PWD", "PLATFORMIO_PROJECT_DIR"):
         if is_platformio_project(project_dir):
             break
         if os.getenv(name):
             project_dir = os.getenv(name)
 
     with fs.cd(project_dir):
-        return _debug_in_project_dir(
+        project_config = ProjectConfig.get_instance(project_conf)
+        project_config.validate(envs=[environment] if environment else None)
+        env_name = environment or helpers.get_default_debug_env(project_config)
+
+        if not interface:
+            return helpers.predebug_project(
+                ctx, project_dir, project_config, env_name, False, verbose
+            )
+
+        configure_args = (
             ctx,
-            project_dir,
-            project_conf,
-            environment,
+            project_config,
+            env_name,
             load_mode,
             verbose,
-            interface,
             __unprocessed,
         )
+        if helpers.is_gdbmi_mode():
+            os.environ["PLATFORMIO_DISABLE_PROGRESSBAR"] = "true"
+            stream = helpers.GDBMIConsoleStream()
+            with proc.capture_std_streams(stream):
+                debug_config = _configure(*configure_args)
+            stream.close()
+        else:
+            debug_config = _configure(*configure_args)
 
+        _run(project_dir, debug_config, __unprocessed)
 
-def _debug_in_project_dir(
-    ctx,
-    project_dir,
-    project_conf,
-    environment,
-    load_mode,
-    verbose,
-    interface,
-    __unprocessed,
-):
-    project_config = ProjectConfig.get_instance(project_conf)
-    project_config.validate(envs=[environment] if environment else None)
-    env_name = environment or helpers.get_default_debug_env(project_config)
-
-    if not interface:
-        return helpers.predebug_project(
-            ctx, project_dir, project_config, env_name, False, verbose
-        )
+    return None
 
-    env_options = project_config.items(env=env_name, as_dict=True)
-    if "platform" not in env_options:
-        raise ProjectEnvsNotAvailableError()
 
+def _configure(ctx, project_config, env_name, load_mode, verbose, __unprocessed):
+    platform = PlatformFactory.new(
+        project_config.get(f"env:{env_name}", "platform"), autoinstall=True
+    )
     debug_config = DebugConfigFactory.new(
-        PlatformFactory.new(env_options["platform"], autoinstall=True),
+        platform,
         project_config,
         env_name,
     )
-
     if "--version" in __unprocessed:
-        return subprocess.run(
-            [debug_config.client_executable_path, "--version"], check=True
+        raise ReturnErrorCode(
+            subprocess.run(
+                [debug_config.client_executable_path, "--version"], check=True
+            ).returncode
         )
 
     try:
         fs.ensure_udev_rules()
     except exception.InvalidUdevRules as exc:
-        click.echo(
-            helpers.escape_gdbmi_stream("~", str(exc) + "\n")
-            if helpers.is_gdbmi_mode()
-            else str(exc) + "\n",
-            nl=False,
-        )
+        click.echo(str(exc))
 
     rebuild_prog = False
     preload = debug_config.load_cmds == ["preload"]
     load_mode = load_mode or debug_config.load_mode
     if load_mode == "always":
         rebuild_prog = preload or not helpers.has_debug_symbols(
             debug_config.program_path
@@ -153,40 +145,29 @@
         rebuild_prog = True
 
     if preload or (not rebuild_prog and load_mode != "always"):
         # don't load firmware through debug server
         debug_config.load_cmds = []
 
     if rebuild_prog:
-        if helpers.is_gdbmi_mode():
-            click.echo(
-                helpers.escape_gdbmi_stream(
-                    "~", "Preparing firmware for debugging...\n"
-                ),
-                nl=False,
-            )
-            stream = helpers.GDBMIConsoleStream()
-            with proc.capture_std_streams(stream):
-                helpers.predebug_project(
-                    ctx, project_dir, project_config, env_name, preload, verbose
-                )
-            stream.close()
-        else:
-            click.echo("Preparing firmware for debugging...")
-            helpers.predebug_project(
-                ctx, project_dir, project_config, env_name, preload, verbose
-            )
-
+        click.echo("Preparing firmware for debugging...")
+        helpers.predebug_project(
+            ctx, os.getcwd(), project_config, env_name, preload, verbose
+        )
         # save SHA sum of newly created prog
         if load_mode == "modified":
             helpers.is_prog_obsolete(debug_config.program_path)
 
     if not os.path.isfile(debug_config.program_path):
         raise DebugInvalidOptionsError("Program/firmware is missed")
 
+    return debug_config
+
+
+def _run(project_dir, debug_config, __unprocessed):
     loop = asyncio.ProactorEventLoop() if IS_WINDOWS else asyncio.get_event_loop()
     asyncio.set_event_loop(loop)
 
     client = GDBClientProcess(project_dir, debug_config)
     coro = client.run(__unprocessed)
     try:
         signal.signal(signal.SIGINT, signal.SIG_IGN)
@@ -195,9 +176,7 @@
             client.close()
             # an issue with `asyncio` executor and STIDIN,
             # it cannot be closed gracefully
             proc.force_exit()
     finally:
         client.close()
         loop.close()
-
-    return True
```

### Comparing `platformio-6.1.6/platformio/debug/config/__init__.py` & `platformio-6.1.7/platformio/debug/config/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/debug/config/base.py` & `platformio-6.1.7/platformio/debug/config/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,17 +142,17 @@
     def server_ready_pattern(self):
         return self.env_options.get(
             "debug_server_ready_pattern", (self.server or {}).get("ready_pattern")
         )
 
     def _load_build_data(self):
         data = load_build_metadata(os.getcwd(), self.env_name, cache=True, debug=True)
-        if data:
-            return data
-        raise DebugInvalidOptionsError("Could not load a build configuration")
+        if not data:
+            raise DebugInvalidOptionsError("Could not load a build configuration")
+        return data
 
     def _configure_server(self):
         # user disabled server in platformio.ini
         if "debug_server" in self.env_options and not self.env_options.get(
             "debug_server"
         ):
             return None
```

### Comparing `platformio-6.1.6/platformio/debug/config/blackmagic.py` & `platformio-6.1.7/platformio/debug/config/blackmagic.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 
 from platformio.debug.config.base import DebugConfigBase
 from platformio.debug.exception import DebugInvalidOptionsError
 from platformio.device.finder import SerialPortFinder, is_pattern_port
 
 
 class BlackmagicDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
     set language c
     set *0xE000ED0C = 0x05FA0004
     set $busy = (*0xE000ED0C & 0x4)
     while ($busy)
         set $busy = (*0xE000ED0C & 0x4)
```

### Comparing `platformio-6.1.6/platformio/debug/config/factory.py` & `platformio-6.1.7/platformio/debug/config/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/debug/config/generic.py` & `platformio-6.1.7/platformio/debug/config/generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio.debug.config.base import DebugConfigBase
 
 
 class GenericDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
     monitor reset halt
 end
 
 define pio_reset_run_target
     monitor reset
```

### Comparing `platformio-6.1.6/platformio/debug/config/jlink.py` & `platformio-6.1.7/platformio/debug/config/jlink.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio.debug.config.base import DebugConfigBase
 
 
 class JlinkDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
     monitor reset
     monitor halt
 end
 
 define pio_reset_run_target
```

### Comparing `platformio-6.1.6/platformio/debug/config/mspdebug.py` & `platformio-6.1.7/platformio/debug/config/mspdebug.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio.debug.config.base import DebugConfigBase
 
 
 class MspdebugDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
 end
 
 define pio_reset_run_target
 end
```

### Comparing `platformio-6.1.6/platformio/debug/config/native.py` & `platformio-6.1.7/platformio/debug/config/native.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from platformio.compat import IS_WINDOWS
 from platformio.debug.config.base import DebugConfigBase
 
 
 class NativeDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
 end
 
 define pio_reset_run_target
 end
```

### Comparing `platformio-6.1.6/platformio/debug/config/qemu.py` & `platformio-6.1.7/platformio/debug/config/qemu.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio.debug.config.base import DebugConfigBase
 
 
 class QemuDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
     monitor system_reset
 end
 
 define pio_reset_run_target
     monitor system_reset
```

### Comparing `platformio-6.1.6/platformio/debug/config/renode.py` & `platformio-6.1.7/platformio/debug/config/renode.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio.debug.config.base import DebugConfigBase
 
 
 class RenodeDebugConfig(DebugConfigBase):
-
     GDB_INIT_SCRIPT = """
 define pio_reset_halt_target
     monitor machine Reset
     $LOAD_CMDS
     monitor start
 end
```

### Comparing `platformio-6.1.6/platformio/debug/exception.py` & `platformio-6.1.7/platformio/debug/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class DebugError(PlatformioException):
     pass
 
 
 class DebugSupportError(DebugError, UserSideException):
-
     MESSAGE = (
         "Currently, PlatformIO does not support debugging for `{0}`.\n"
         "Please request support at https://github.com/platformio/"
         "platformio-core/issues \nor visit -> https://docs.platformio.org"
         "/page/plus/debugging.html"
     )
```

### Comparing `platformio-6.1.6/platformio/debug/helpers.py` & `platformio-6.1.7/platformio/debug/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 from platformio.test.helpers import list_test_names
 from platformio.test.result import TestSuite
 from platformio.test.runners.base import TestRunnerOptions
 from platformio.test.runners.factory import TestRunnerFactory
 
 
 class GDBMIConsoleStream(BytesIO):  # pylint: disable=too-few-public-methods
-
     STDOUT = sys.stdout
 
     def write(self, text):
         self.STDOUT.write(escape_gdbmi_stream("~", text))
         self.STDOUT.flush()
 
 
@@ -87,15 +86,15 @@
                 % (debug_testname, ", ".join(test_names))
             )
         print_processing_header(env_name, project_config, verbose)
         test_runner = TestRunnerFactory.new(
             TestSuite(env_name, debug_testname),
             project_config,
             TestRunnerOptions(
-                verbose=verbose,
+                verbose=3 if verbose else 0,
                 without_building=False,
                 without_debugging=False,
                 without_uploading=not preload,
                 without_testing=True,
             ),
         )
         test_runner.start(ctx)
```

### Comparing `platformio-6.1.6/platformio/debug/process/__init__.py` & `platformio-6.1.7/platformio/debug/process/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/debug/process/base.py` & `platformio-6.1.7/platformio/debug/process/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         if self._is_exited:
             return
         self.factory.process_exited()
         self._is_exited = True
 
 
 class DebugBaseProcess:
-
     STDOUT_CHUNK_SIZE = 2048
     LOG_FILE = None
 
     def __init__(self):
         self.transport = None
         self._is_running = False
         self._last_activity = 0
```

### Comparing `platformio-6.1.6/platformio/debug/process/client.py` & `platformio-6.1.7/platformio/debug/process/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/debug/process/gdb.py` & `platformio-6.1.7/platformio/debug/process/gdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from platformio import telemetry
 from platformio.compat import aio_get_running_loop, is_bytes
 from platformio.debug import helpers
 from platformio.debug.process.client import DebugClientProcess
 
 
 class GDBClientProcess(DebugClientProcess):
-
     PIO_SRC_NAME = ".pioinit"
     INIT_COMPLETED_BANNER = "PlatformIO: Initialization completed"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._target_is_running = False
         self._errors_buffer = b""
```

### Comparing `platformio-6.1.6/platformio/debug/process/server.py` & `platformio-6.1.7/platformio/debug/process/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from platformio.debug.exception import DebugInvalidOptionsError
 from platformio.debug.helpers import escape_gdbmi_stream, is_gdbmi_mode
 from platformio.debug.process.base import DebugBaseProcess
 from platformio.proc import where_is_program
 
 
 class DebugServerProcess(DebugBaseProcess):
-
     STD_BUFFER_SIZE = 1024
 
     def __init__(self, debug_config):
         super().__init__()
         self.debug_config = debug_config
         self._ready = False
         self._std_buffer = {"out": b"", "err": b""}
```

### Comparing `platformio-6.1.6/platformio/device/__init__.py` & `platformio-6.1.7/platformio/device/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/cli.py` & `platformio-6.1.7/platformio/device/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/finder.py` & `platformio-6.1.7/platformio/device/finder.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/list/__init__.py` & `platformio-6.1.7/platformio/device/list/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/list/command.py` & `platformio-6.1.7/platformio/device/list/command.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/list/util.py` & `platformio-6.1.7/platformio/device/list/util.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/__init__.py` & `platformio-6.1.7/platformio/device/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/command.py` & `platformio-6.1.7/platformio/device/monitor/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     is_flag=True,
     help="Disable automatic reconnection if the established connection fails",
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option(
     "-e",
     "--environment",
     help="Load configuration from `platformio.ini` and the specified environment",
 )
 def device_monitor_cmd(**options):
@@ -128,32 +128,32 @@
             board_config=platform.board_config(project_options.get("board"))
             if platform and project_options.get("board")
             else None,
             upload_protocol=project_options.get("upload_protocol"),
             ensure_ready=True,
         ).find(initial_port=options["port"])
 
-    if options["menu_char"] == options["exit_char"]:
-        raise exception.UserSideException(
-            "--exit-char can not be the same as --menu-char"
-        )
-
-    # check for unknown filters
-    if options["filters"]:
-        known_filters = set(get_available_filters())
-        unknown_filters = set(options["filters"]) - known_filters
-        if unknown_filters:
-            options["filters"] = list(known_filters & set(options["filters"]))
-            click.secho(
-                ("Warning! Skipping unknown filters `%s`. Known filters are `%s`")
-                % (", ".join(unknown_filters), ", ".join(sorted(known_filters))),
-                fg="yellow",
+        if options["menu_char"] == options["exit_char"]:
+            raise exception.UserSideException(
+                "--exit-char can not be the same as --menu-char"
             )
 
-    start_terminal(options)
+        # check for unknown filters
+        if options["filters"]:
+            known_filters = set(get_available_filters())
+            unknown_filters = set(options["filters"]) - known_filters
+            if unknown_filters:
+                options["filters"] = list(known_filters & set(options["filters"]))
+                click.secho(
+                    ("Warning! Skipping unknown filters `%s`. Known filters are `%s`")
+                    % (", ".join(unknown_filters), ", ".join(sorted(known_filters))),
+                    fg="yellow",
+                )
+
+        start_terminal(options)
 
 
 def get_project_options(environment=None):
     config = ProjectConfig.get_instance()
     config.validate(envs=[environment] if environment else None)
     environment = environment or config.get_default_env()
     return config.items(env=environment, as_dict=True)
```

### Comparing `platformio-6.1.6/platformio/device/monitor/filters/__init__.py` & `platformio-6.1.7/platformio/device/monitor/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/filters/base.py` & `platformio-6.1.7/platformio/device/monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/filters/hexlify.py` & `platformio-6.1.7/platformio/device/monitor/filters/hexlify.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/filters/log2file.py` & `platformio-6.1.7/platformio/device/monitor/filters/log2file.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,30 +9,32 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-import os.path
+import os
 from datetime import datetime
 
 from platformio.device.monitor.filters.base import DeviceMonitorFilterBase
 
 
 class LogToFile(DeviceMonitorFilterBase):
     NAME = "log2file"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._log_fp = None
 
     def __call__(self):
-        log_file_name = "platformio-device-monitor-%s.log" % datetime.now().strftime(
-            "%y%m%d-%H%M%S"
+        if not os.path.isdir("logs"):
+            os.makedirs("logs")
+        log_file_name = os.path.join(
+            "logs", "device-monitor-%s.log" % datetime.now().strftime("%y%m%d-%H%M%S")
         )
         print("--- Logging an output to %s" % os.path.abspath(log_file_name))
         # pylint: disable=consider-using-with
         self._log_fp = io.open(log_file_name, "w", encoding="utf-8")
         return self
 
     def __del__(self):
```

### Comparing `platformio-6.1.6/platformio/device/monitor/filters/send_on_enter.py` & `platformio-6.1.7/platformio/device/monitor/filters/send_on_enter.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/filters/time.py` & `platformio-6.1.7/platformio/device/monitor/filters/time.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/device/monitor/terminal.py` & `platformio-6.1.7/platformio/device/monitor/terminal.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,17 +140,16 @@
         # no port given on command line -> ask user now
         if port is None or port == "-":
             try:
                 port = miniterm.ask_for_port()
             except KeyboardInterrupt as exc:
                 click.echo("", err=True)
                 raise UserSideException("User aborted and port is not given") from exc
-            else:
-                if not port:
-                    raise UserSideException("Port is not given")
+            if not port:
+                raise UserSideException("Port is not given")
         try:
             serial_instance = serial.serial_for_url(
                 port,
                 options["baud"],
                 parity=options["parity"],
                 rtscts=options["rtscts"],
                 xonxoff=options["xonxoff"],
```

### Comparing `platformio-6.1.6/platformio/exception.py` & `platformio-6.1.7/platformio/exception.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,124 +10,101 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 class PlatformioException(Exception):
-
     MESSAGE = None
 
     def __str__(self):  # pragma: no cover
         if self.MESSAGE:
             # pylint: disable=not-an-iterable
             return self.MESSAGE.format(*self.args)
 
         return super().__str__()
 
 
 class ReturnErrorCode(PlatformioException):
-
     MESSAGE = "{0}"
 
 
 class UserSideException(PlatformioException):
     pass
 
 
 class AbortedByUser(UserSideException):
-
     MESSAGE = "Aborted by user"
 
 
 #
 # UDEV Rules
 #
 
 
 class InvalidUdevRules(UserSideException):
     pass
 
 
 class MissedUdevRules(InvalidUdevRules):
-
     MESSAGE = (
         "Warning! Please install `99-platformio-udev.rules`. \nMore details: "
         "https://docs.platformio.org/en/latest/core/installation/udev-rules.html"
     )
 
 
 class OutdatedUdevRules(InvalidUdevRules):
-
     MESSAGE = (
         "Warning! Your `{0}` are outdated. Please update or reinstall them."
         "\nMore details: "
         "https://docs.platformio.org/en/latest/core/installation/udev-rules.html"
     )
 
 
 #
 # Misc
 #
 
 
 class GetSerialPortsError(PlatformioException):
-
     MESSAGE = "No implementation for your platform ('{0}') available"
 
 
 class GetLatestVersionError(PlatformioException):
-
     MESSAGE = "Can not retrieve the latest PlatformIO version"
 
 
 class InvalidSettingName(UserSideException):
-
     MESSAGE = "Invalid setting with the name '{0}'"
 
 
 class InvalidSettingValue(UserSideException):
-
     MESSAGE = "Invalid value '{0}' for the setting '{1}'"
 
 
 class InvalidJSONFile(PlatformioException):
-
     MESSAGE = "Could not load broken JSON: {0}"
 
 
 class CIBuildEnvsEmpty(UserSideException):
-
     MESSAGE = (
         "Can't find PlatformIO build environments.\n"
         "Please specify `--board` or path to `platformio.ini` with "
         "predefined environments using `--project-conf` option"
     )
 
 
-class UpgradeError(PlatformioException):
-
-    MESSAGE = """{0}
-
-* Upgrade using `pip install -U platformio`
-* Try different installation/upgrading steps:
-  https://docs.platformio.org/page/installation.html
-"""
-
-
 class HomeDirPermissionsError(UserSideException):
-
     MESSAGE = (
         "The directory `{0}` or its parent directory is not owned by the "
         "current user and PlatformIO can not store configuration data.\n"
         "Please check the permissions and owner of that directory.\n"
         "Otherwise, please remove manually `{0}` directory and PlatformIO "
         "will create new from the current user."
     )
 
 
 class CygwinEnvDetected(PlatformioException):
-
     MESSAGE = (
         "PlatformIO does not work within Cygwin environment. "
         "Use native Terminal instead."
     )
```

### Comparing `platformio-6.1.6/platformio/fs.py` & `platformio-6.1.7/platformio/fs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import re
 import shutil
 import stat
 import sys
 
 import click
 
-from platformio import exception, proc
+from platformio import exception
 from platformio.compat import IS_WINDOWS
 
 
 class cd:
     def __init__(self, new_path):
         self.new_path = new_path
         self.prev_path = os.getcwd()
@@ -177,46 +177,27 @@
     src_filter = src_filter or ""
     if isinstance(src_filter, (list, tuple)):
         src_filter = " ".join(src_filter)
 
     result = set()
     # correct fs directory separator
     src_filter = src_filter.replace("/", os.sep).replace("\\", os.sep)
-    for (action, pattern) in re.findall(r"(\+|\-)<([^>]+)>", src_filter):
+    for action, pattern in re.findall(r"(\+|\-)<([^>]+)>", src_filter):
         candidates = _find_candidates(pattern)
         if action == "+":
             result |= candidates
         else:
             result -= candidates
     return sorted(list(result))
 
 
 def to_unix_path(path):
     if not IS_WINDOWS or not path:
         return path
-    return re.sub(r"[\\]+", "/", path)
-
-
-def normalize_path(path):
-    path = os.path.abspath(path)
-    if not IS_WINDOWS or not path.startswith("\\\\"):
-        return path
-    try:
-        result = proc.exec_command(["net", "use"])
-        if result["returncode"] != 0:
-            return path
-        share_re = re.compile(r"\s([A-Z]\:)\s+(\\\\[^\s]+)")
-        for line in result["out"].split("\n"):
-            share = share_re.search(line)
-            if not share:
-                continue
-            path = path.replace(share.group(2), share.group(1))
-    except OSError:
-        pass
-    return path
+    return path.replace("\\", "/")
 
 
 def expanduser(path):
     """
     Be compatible with Python 3.8, on Windows skip HOME and check for USERPROFILE
     """
     if not IS_WINDOWS or not path.startswith("~") or "USERPROFILE" not in os.environ:
```

### Comparing `platformio-6.1.6/platformio/home/__init__.py` & `platformio-6.1.7/platformio/home/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/home/cli.py` & `platformio-6.1.7/platformio/home/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import mimetypes
+import socket
 
 import click
 
-from platformio.home.helpers import is_port_used
+from platformio.compat import IS_WINDOWS
 from platformio.home.run import run_server
 from platformio.package.manager.core import get_core_package_dir
 
 
 @click.command("home", short_help="GUI to manage PlatformIO")
 @click.option("--port", type=int, default=8008, help="HTTP port, default=8008")
 @click.option(
@@ -91,7 +92,27 @@
     run_server(
         host=host,
         port=port,
         no_open=no_open,
         shutdown_timeout=shutdown_timeout,
         home_url=home_url,
     )
+
+
+def is_port_used(host, port):
+    socket.setdefaulttimeout(1)
+    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+    if IS_WINDOWS:
+        try:
+            s.bind((host, port))
+            s.close()
+            return False
+        except (OSError, socket.error):
+            pass
+    else:
+        try:
+            s.connect((host, port))
+            s.close()
+        except socket.error:
+            return False
+
+    return True
```

### Comparing `platformio-6.1.6/platformio/home/helpers.py` & `platformio-6.1.7/platformio/registry/access/commands/public.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,37 +8,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import socket
+import click
 
-from platformio import util
-from platformio.compat import IS_WINDOWS
-from platformio.proc import where_is_program
+from platformio.registry.access.validate import validate_urn
+from platformio.registry.client import RegistryClient
 
 
-@util.memoized(expire="60s")
-def get_core_fullpath():
-    return where_is_program("platformio" + (".exe" if IS_WINDOWS else ""))
-
-
-def is_port_used(host, port):
-    socket.setdefaulttimeout(1)
-    s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    if IS_WINDOWS:
-        try:
-            s.bind((host, port))
-            s.close()
-            return False
-        except (OSError, socket.error):
-            pass
-    else:
-        try:
-            s.connect((host, port))
-            s.close()
-        except socket.error:
-            return False
-
-    return True
+@click.command("public", short_help="Make resource public")
+@click.argument(
+    "urn",
+    callback=lambda _, __, value: validate_urn(value),
+)
+@click.option("--urn-type", type=click.Choice(["prn:reg:pkg"]), default="prn:reg:pkg")
+def access_public_cmd(urn, urn_type):  # pylint: disable=unused-argument
+    client = RegistryClient()
+    client.update_resource(urn=urn, private=0)
+    return click.secho(
+        "The resource %s has been successfully updated." % urn,
+        fg="green",
+    )
```

### Comparing `platformio-6.1.6/platformio/home/rpc/__init__.py` & `platformio-6.1.7/platformio/home/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/__init__.py` & `platformio-6.1.7/platformio/home/rpc/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/account.py` & `platformio-6.1.7/platformio/home/rpc/handlers/account.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ajsonrpc.core import JSONRPC20DispatchException
 
 from platformio.account.client import AccountClient
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 
 
-class AccountRPC:
+class AccountRPC(BaseRPCHandler):
     @staticmethod
     def call_client(method, *args, **kwargs):
         try:
             client = AccountClient()
             return getattr(client, method)(*args, **kwargs)
         except Exception as exc:  # pylint: disable=bare-except
             raise JSONRPC20DispatchException(
-                code=4003, message="PIO Account Call Error", data=str(exc)
+                code=5000, message="PIO Account Call Error", data=str(exc)
             ) from exc
```

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/app.py` & `platformio-6.1.7/platformio/home/rpc/handlers/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from pathlib import Path
 
 from platformio import __version__, app, fs, util
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.project.config import ProjectConfig
 from platformio.project.helpers import is_platformio_project
 
 
-class AppRPC:
-
+class AppRPC(BaseRPCHandler):
     IGNORE_STORAGE_KEYS = [
         "cid",
         "coreVersion",
         "coreSystype",
         "coreCaller",
         "coreSettings",
         "homeDir",
```

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/ide.py` & `platformio-6.1.7/platformio/home/rpc/handlers/ide.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
 import time
 from pathlib import Path
 
 from ajsonrpc.core import JSONRPC20DispatchException
 
 from platformio.compat import aio_get_running_loop
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 
 
-class IDERPC:
-
+class IDERPC(BaseRPCHandler):
     COMMAND_TIMEOUT = 1.5  # in seconds
 
     def __init__(self):
         self._ide_queue = []
         self._cmd_queue = {}
 
     async def listen_commands(self):
@@ -47,19 +47,20 @@
         aio_get_running_loop().call_later(
             self.COMMAND_TIMEOUT + 0.1, self._process_commands
         )
         return await self._cmd_queue[cmd_id]["future"]
 
     def on_command_result(self, cmd_id, value):
         if cmd_id not in self._cmd_queue:
-            return
+            return False
         if self._cmd_queue[cmd_id]["method"] == "get_pio_project_dirs":
             value = [str(Path(p).resolve()) for p in value]
         self._cmd_queue[cmd_id]["future"].set_result(value)
         del self._cmd_queue[cmd_id]
+        return True
 
     def _process_commands(self):
         for cmd_id in list(self._cmd_queue):
             cmd_data = self._cmd_queue[cmd_id]
             if cmd_data["future"].done():
                 del self._cmd_queue[cmd_id]
                 continue
```

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/misc.py` & `platformio-6.1.7/platformio/home/rpc/handlers/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 # limitations under the License.
 
 import json
 import time
 
 from platformio.cache import ContentCache
 from platformio.compat import aio_create_task
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.home.rpc.handlers.os import OSRPC
 
 
-class MiscRPC:
+class MiscRPC(BaseRPCHandler):
     async def load_latest_tweets(self, data_url):
         cache_key = ContentCache.key_from_args(data_url, "tweets")
         cache_valid = "180d"
         with ContentCache() as cc:
             cache_data = cc.get(cache_key)
             if cache_data:
                 cache_data = json.loads(cache_data)
```

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/os.py` & `platformio-6.1.7/platformio/home/rpc/handlers/os.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 
 import click
 from starlette.concurrency import run_in_threadpool
 
 from platformio import fs
 from platformio.cache import ContentCache
 from platformio.device.list.util import list_logical_devices
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.http import HTTPSession, ensure_internet_on
 
 
 class HTTPAsyncSession(HTTPSession):
     async def request(  # pylint: disable=signature-differs,invalid-overridden-method
         self, *args, **kwargs
     ):
         func = super().request
         return await run_in_threadpool(func, *args, **kwargs)
 
 
-class OSRPC:
+class OSRPC(BaseRPCHandler):
     @staticmethod
     async def fetch_content(url, data=None, headers=None, cache_valid=None):
         if not headers:
             headers = {
                 "User-Agent": (
                     "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_12_6) "
                     "AppleWebKit/603.3.8 (KHTML, like Gecko) Version/10.1.2 "
@@ -86,14 +87,22 @@
         return click.launch(path, locate=True)
 
     @staticmethod
     def open_file(path):
         return click.launch(path)
 
     @staticmethod
+    def call_path_module_func(name, args, **kwargs):
+        return getattr(os.path, name)(*args, **kwargs)
+
+    @staticmethod
+    def get_path_separator():
+        return os.sep
+
+    @staticmethod
     def is_file(path):
         return os.path.isfile(path)
 
     @staticmethod
     def is_dir(path):
         return os.path.isdir(path)
 
@@ -152,13 +161,8 @@
                 items.append((item, item_is_dir))
             except OSError:
                 pass
         return sorted(items, key=cmp_to_key(_cmp))
 
     @staticmethod
     def get_logical_devices():
-        items = []
-        for item in list_logical_devices():
-            if item["name"]:
-                item["name"] = item["name"]
-            items.append(item)
-        return items
+        return list_logical_devices()
```

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/project.py` & `platformio-6.1.7/platformio/home/rpc/handlers/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 import shutil
 import time
 
+import semantic_version
 from ajsonrpc.core import JSONRPC20DispatchException
 
-from platformio import exception, fs
+from platformio import app, exception, fs
 from platformio.home.rpc.handlers.app import AppRPC
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.home.rpc.handlers.piocore import PIOCoreRPC
 from platformio.package.manager.platform import PlatformPackageManager
 from platformio.project.config import ProjectConfig
 from platformio.project.exception import ProjectError
 from platformio.project.helpers import get_project_dir, is_platformio_project
 from platformio.project.integration.generator import ProjectGenerator
 from platformio.project.options import get_config_options_schema
 
 
-class ProjectRPC:
+class ProjectRPC(BaseRPCHandler):
     @staticmethod
     def config_call(init_kwargs, method, *args):
         assert isinstance(init_kwargs, dict)
         assert "path" in init_kwargs
         project_dir = get_project_dir()
         if os.path.isfile(init_kwargs["path"]):
             project_dir = os.path.dirname(init_kwargs["path"])
@@ -180,91 +182,25 @@
                     "items": sorted(items, key=lambda item: item["name"]),
                 }
             )
         return sorted(result, key=lambda data: data["platform"]["title"])
 
     async def init(self, board, framework, project_dir):
         assert project_dir
-        state = AppRPC.load_state()
         if not os.path.isdir(project_dir):
             os.makedirs(project_dir)
-        args = ["init", "--board", board]
+        args = ["init", "--board", board, "--sample-code"]
         if framework:
             args.extend(["--project-option", "framework = %s" % framework])
-        if (
-            state["storage"]["coreCaller"]
-            and state["storage"]["coreCaller"] in ProjectGenerator.get_supported_ides()
-        ):
-            args.extend(["--ide", state["storage"]["coreCaller"]])
+        ide = app.get_session_var("caller_id")
+        if ide in ProjectGenerator.get_supported_ides():
+            args.extend(["--ide", ide])
         await PIOCoreRPC.call(
             args, options={"cwd": project_dir, "force_subprocess": True}
         )
-        return self._generate_project_main(project_dir, board, framework)
-
-    @staticmethod
-    def _generate_project_main(project_dir, board, framework):
-        main_content = None
-        if framework == "arduino":
-            main_content = "\n".join(
-                [
-                    "#include <Arduino.h>",
-                    "",
-                    "void setup() {",
-                    "  // put your setup code here, to run once:",
-                    "}",
-                    "",
-                    "void loop() {",
-                    "  // put your main code here, to run repeatedly:",
-                    "}",
-                    "",
-                ]
-            )
-        elif framework == "mbed":
-            main_content = "\n".join(
-                [
-                    "#include <mbed.h>",
-                    "",
-                    "int main() {",
-                    "",
-                    "  // put your setup code here, to run once:",
-                    "",
-                    "  while(1) {",
-                    "    // put your main code here, to run repeatedly:",
-                    "  }",
-                    "}",
-                    "",
-                ]
-            )
-        if not main_content:
-            return project_dir
-
-        is_cpp_project = True
-        pm = PlatformPackageManager()
-        try:
-            board = pm.board_config(board)
-            platforms = board.get("platforms", board.get("platform"))
-            if not isinstance(platforms, list):
-                platforms = [platforms]
-            c_based_platforms = ["intel_mcs51", "ststm8"]
-            is_cpp_project = not set(platforms) & set(c_based_platforms)
-        except exception.PlatformioException:
-            pass
-
-        with fs.cd(project_dir):
-            config = ProjectConfig()
-            src_dir = config.get("platformio", "src_dir")
-            main_path = os.path.join(
-                src_dir, "main.%s" % ("cpp" if is_cpp_project else "c")
-            )
-            if os.path.isfile(main_path):
-                return project_dir
-            if not os.path.isdir(src_dir):
-                os.makedirs(src_dir)
-            with open(main_path, mode="w", encoding="utf8") as fp:
-                fp.write(main_content.strip())
         return project_dir
 
     @staticmethod
     async def import_arduino(board, use_arduino_libs, arduino_project_dir):
         board = str(board)
         # don't import PIO Project
         if is_platformio_project(arduino_project_dir):
@@ -292,19 +228,17 @@
             os.makedirs(project_dir)
         args = ["init", "--board", board]
         args.extend(["--project-option", "framework = arduino"])
         if use_arduino_libs:
             args.extend(
                 ["--project-option", "lib_extra_dirs = ~/Documents/Arduino/libraries"]
             )
-        if (
-            state["storage"]["coreCaller"]
-            and state["storage"]["coreCaller"] in ProjectGenerator.get_supported_ides()
-        ):
-            args.extend(["--ide", state["storage"]["coreCaller"]])
+        ide = app.get_session_var("caller_id")
+        if ide in ProjectGenerator.get_supported_ides():
+            args.extend(["--ide", ide])
         await PIOCoreRPC.call(
             args, options={"cwd": project_dir, "force_subprocess": True}
         )
         with fs.cd(project_dir):
             config = ProjectConfig()
             src_dir = config.get("platformio", "src_dir")
             if os.path.isdir(src_dir):
@@ -320,18 +254,54 @@
             )
         new_project_dir = os.path.join(
             AppRPC.load_state()["storage"]["projectsDir"],
             time.strftime("%y%m%d-%H%M%S-") + os.path.basename(project_dir),
         )
         shutil.copytree(project_dir, new_project_dir, symlinks=True)
 
-        state = AppRPC.load_state()
         args = ["init"]
-        if (
-            state["storage"]["coreCaller"]
-            and state["storage"]["coreCaller"] in ProjectGenerator.get_supported_ides()
-        ):
-            args.extend(["--ide", state["storage"]["coreCaller"]])
+        ide = app.get_session_var("caller_id")
+        if ide in ProjectGenerator.get_supported_ides():
+            args.extend(["--ide", ide])
         await PIOCoreRPC.call(
             args, options={"cwd": new_project_dir, "force_subprocess": True}
         )
         return new_project_dir
+
+    async def create_empty(self, configuration, options=None):
+        project_dir = os.path.join(configuration["location"], configuration["name"])
+        if not os.path.isdir(project_dir):
+            os.makedirs(project_dir)
+
+        project_options = []
+        platform = configuration["platform"]
+        board = configuration.get("board", {}).get("id")
+        env_name = board or platform["name"]
+        if configuration.get("description"):
+            project_options.append(("description", configuration.get("description")))
+        try:
+            v = semantic_version.Version(platform.get("version"))
+            assert not v.prerelease
+            project_options.append(
+                ("platform", "{name} @ ^{version}".format(**platform))
+            )
+        except (AssertionError, ValueError):
+            project_options.append(
+                ("platform", "{name} @ {version}".format(**platform))
+            )
+        if board:
+            project_options.append(("board", board))
+        if configuration.get("framework"):
+            project_options.append(("framework", configuration["framework"]["name"]))
+
+        args = ["project", "init", "-e", env_name, "--sample-code"]
+        ide = app.get_session_var("caller_id")
+        if ide in ProjectGenerator.get_supported_ides():
+            args.extend(["--ide", ide])
+        for name, value in project_options:
+            args.extend(["-O", f"{name}={value}"])
+
+        envclone = os.environ.copy()
+        envclone["PLATFORMIO_FORCE_ANSI"] = "true"
+        options = options or {}
+        options["spawn"] = {"env": envclone, "cwd": project_dir}
+        return await self.factory.manager.dispatcher["core.exec"](args, options=options)
```

### Comparing `platformio-6.1.6/platformio/home/rpc/handlers/registry.py` & `platformio-6.1.7/platformio/home/rpc/handlers/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from ajsonrpc.core import JSONRPC20DispatchException
+from starlette.concurrency import run_in_threadpool
 
+from platformio.home.rpc.handlers.base import BaseRPCHandler
 from platformio.registry.client import RegistryClient
 
 
-class RegistryRPC:
+class RegistryRPC(BaseRPCHandler):
     @staticmethod
-    def call_client(method, *args, **kwargs):
+    async def call_client(method, *args, **kwargs):
         try:
             client = RegistryClient()
-            return getattr(client, method)(*args, **kwargs)
+            return await run_in_threadpool(getattr(client, method), *args, **kwargs)
         except Exception as exc:  # pylint: disable=bare-except
             raise JSONRPC20DispatchException(
-                code=4003, message="Registry Call Error", data=str(exc)
+                code=5000, message="Registry Call Error", data=str(exc)
             ) from exc
```

### Comparing `platformio-6.1.6/platformio/home/rpc/server.py` & `platformio-6.1.7/platformio/home/rpc/server.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,47 +8,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from urllib.parse import parse_qs
+
 import click
+from ajsonrpc.core import JSONRPC20Error, JSONRPC20Request
 from ajsonrpc.dispatcher import Dispatcher
-from ajsonrpc.manager import AsyncJSONRPCResponseManager
+from ajsonrpc.manager import AsyncJSONRPCResponseManager, JSONRPC20Response
 from starlette.endpoints import WebSocketEndpoint
 
 from platformio.compat import aio_create_task, aio_get_running_loop
+from platformio.http import InternetConnectionError
 from platformio.proc import force_exit
 
 
 class JSONRPCServerFactoryBase:
-
     connection_nums = 0
     shutdown_timer = None
 
     def __init__(self, shutdown_timeout=0):
         self.shutdown_timeout = shutdown_timeout
         self.manager = AsyncJSONRPCResponseManager(
             Dispatcher(), is_server_error_verbose=True
         )
+        self._clients = {}
 
     def __call__(self, *args, **kwargs):
         raise NotImplementedError
 
     def add_object_handler(self, handler, namespace):
+        handler.factory = self
         self.manager.dispatcher.add_object(handler, prefix="%s." % namespace)
 
-    def on_client_connect(self):
+    def on_client_connect(self, connection, actor=None):
+        self._clients[connection] = {"actor": actor}
         self.connection_nums += 1
         if self.shutdown_timer:
             self.shutdown_timer.cancel()
             self.shutdown_timer = None
 
-    def on_client_disconnect(self):
+    def on_client_disconnect(self, connection):
+        if connection in self._clients:
+            del self._clients[connection]
         self.connection_nums -= 1
         if self.connection_nums < 1:
             self.connection_nums = 0
 
         if self.connection_nums == 0:
             self.shutdown_by_timeout()
 
@@ -63,35 +71,56 @@
             click.echo("Automatically shutdown server on timeout")
             force_exit()
 
         self.shutdown_timer = aio_get_running_loop().call_later(
             self.shutdown_timeout, _auto_shutdown_server
         )
 
+    async def notify_clients(self, method, params=None, actor=None):
+        for client, options in self._clients.items():
+            if actor and options["actor"] != actor:
+                continue
+            request = JSONRPC20Request(method, params, is_notification=True)
+            await client.send_text(self.manager.serialize(request.body))
+        return True
+
 
 class WebSocketJSONRPCServerFactory(JSONRPCServerFactoryBase):
     def __call__(self, *args, **kwargs):
         ws = WebSocketJSONRPCServer(*args, **kwargs)
         ws.factory = self
         return ws
 
 
 class WebSocketJSONRPCServer(WebSocketEndpoint):
     encoding = "text"
     factory: WebSocketJSONRPCServerFactory = None
 
     async def on_connect(self, websocket):
         await websocket.accept()
-        self.factory.on_client_connect()  # pylint: disable=no-member
+        qs = parse_qs(self.scope.get("query_string", b""))
+        actors = qs.get(b"actor")
+        self.factory.on_client_connect(  # pylint: disable=no-member
+            websocket, actor=actors[0].decode() if actors else None
+        )
 
     async def on_receive(self, websocket, data):
         aio_create_task(self._handle_rpc(websocket, data))
 
     async def on_disconnect(self, websocket, close_code):
-        self.factory.on_client_disconnect()  # pylint: disable=no-member
+        self.factory.on_client_disconnect(websocket)  # pylint: disable=no-member
 
     async def _handle_rpc(self, websocket, data):
         # pylint: disable=no-member
         response = await self.factory.manager.get_response_for_payload(data)
         if response.error and response.error.data:
             click.secho("Error: %s" % response.error.data, fg="red", err=True)
+            if InternetConnectionError.MESSAGE in response.error.data:
+                response = JSONRPC20Response(
+                    id=response.id,
+                    error=JSONRPC20Error(
+                        code=4008,
+                        message="No Internet Connection",
+                        data=response.error.data,
+                    ),
+                )
         await websocket.send_text(self.factory.manager.serialize(response.body))
```

### Comparing `platformio-6.1.6/platformio/home/run.py` & `platformio-6.1.7/platformio/home/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,27 +28,28 @@
 from platformio.exception import PlatformioException
 from platformio.home.rpc.handlers.account import AccountRPC
 from platformio.home.rpc.handlers.app import AppRPC
 from platformio.home.rpc.handlers.ide import IDERPC
 from platformio.home.rpc.handlers.misc import MiscRPC
 from platformio.home.rpc.handlers.os import OSRPC
 from platformio.home.rpc.handlers.piocore import PIOCoreRPC
+from platformio.home.rpc.handlers.platform import PlatformRPC
 from platformio.home.rpc.handlers.project import ProjectRPC
 from platformio.home.rpc.handlers.registry import RegistryRPC
 from platformio.home.rpc.server import WebSocketJSONRPCServerFactory
 from platformio.package.manager.core import get_core_package_dir
 from platformio.proc import force_exit
 
 
 class ShutdownMiddleware:
     def __init__(self, app):
         self.app = app
 
     async def __call__(self, scope, receive, send):
-        if scope["type"] == "http" and b"__shutdown__" in scope.get("query_string", {}):
+        if scope["type"] == "http" and b"__shutdown__" in scope.get("query_string", ""):
             await shutdown_server()
         await self.app(scope, receive, send)
 
 
 async def shutdown_server(_=None):
     aio_get_running_loop().call_later(0.5, force_exit)
     return PlainTextResponse("Server has been shutdown!")
@@ -69,14 +70,15 @@
     ws_rpc_factory.add_object_handler(AccountRPC(), namespace="account")
     ws_rpc_factory.add_object_handler(AppRPC(), namespace="app")
     ws_rpc_factory.add_object_handler(IDERPC(), namespace="ide")
     ws_rpc_factory.add_object_handler(MiscRPC(), namespace="misc")
     ws_rpc_factory.add_object_handler(OSRPC(), namespace="os")
     ws_rpc_factory.add_object_handler(PIOCoreRPC(), namespace="core")
     ws_rpc_factory.add_object_handler(ProjectRPC(), namespace="project")
+    ws_rpc_factory.add_object_handler(PlatformRPC(), namespace="platform")
     ws_rpc_factory.add_object_handler(RegistryRPC(), namespace="registry")
 
     path = urlparse(home_url).path
     routes = [
         WebSocketRoute(path + "wsrpc", ws_rpc_factory, name="wsrpc"),
         Route(path + "__shutdown__", shutdown_server, methods=["POST"]),
         Mount(path, StaticFiles(directory=contrib_dir, html=True), name="static"),
```

### Comparing `platformio-6.1.6/platformio/http.py` & `platformio-6.1.7/platformio/http.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
         self.message = message
         self.response = response
 
     def __str__(self):  # pragma: no cover
         return self.message
 
 
-class InternetIsOffline(UserSideException):
-
+class InternetConnectionError(UserSideException):
     MESSAGE = (
         "You are not connected to the Internet.\n"
         "PlatformIO needs the Internet connection to"
         " download dependent packages or to work with PlatformIO Account."
     )
 
 
@@ -200,15 +199,15 @@
             pass
     return False
 
 
 def ensure_internet_on(raise_exception=False):
     result = _internet_on()
     if raise_exception and not result:
-        raise InternetIsOffline()
+        raise InternetConnectionError()
     return result
 
 
 def fetch_remote_content(*args, **kwargs):
     with HTTPSession() as s:
         r = s.get(*args, **kwargs)
         r.raise_for_status()
```

### Comparing `platformio-6.1.6/platformio/maintenance.py` & `platformio-6.1.7/platformio/maintenance.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,16 @@
 
 import click
 import semantic_version
 
 from platformio import __version__, app, exception, fs, telemetry
 from platformio.cache import cleanup_content_cache
 from platformio.cli import PlatformioCLI
-from platformio.commands.platform import platform_update as cmd_platform_update
 from platformio.commands.upgrade import get_latest_version
-from platformio.http import HTTPClientError, InternetIsOffline, ensure_internet_on
+from platformio.http import HTTPClientError, InternetConnectionError, ensure_internet_on
 from platformio.package.manager.core import update_core_packages
 from platformio.package.manager.tool import ToolPackageManager
 from platformio.package.meta import PackageSpec
 from platformio.package.version import pepver_to_semver
 from platformio.system.prune import calculate_unnecessary_system_data
 
 
@@ -47,15 +46,15 @@
         return
 
     try:
         check_platformio_upgrade()
         check_prune_system()
     except (
         HTTPClientError,
-        InternetIsOffline,
+        InternetConnectionError,
         exception.GetLatestVersionError,
     ):
         click.secho(
             "Failed to check for PlatformIO upgrades. "
             "Please check your Internet connection.",
             fg="red",
         )
@@ -63,32 +62,31 @@
 
 def on_platformio_exception(e):
     telemetry.on_exception(e)
 
 
 def set_caller(caller=None):
     caller = caller or os.getenv("PLATFORMIO_CALLER")
+    if not caller:
+        if os.getenv("CODESPACES"):
+            caller = "codespaces"
+        elif os.getenv("VSCODE_PID") or os.getenv("VSCODE_NLS_CONFIG"):
+            caller = "vscode"
+        elif os.getenv("GITPOD_WORKSPACE_ID") or os.getenv("GITPOD_WORKSPACE_URL"):
+            caller = "gitpod"
     if caller:
-        return app.set_session_var("caller_id", caller)
-    if os.getenv("CODESPACES"):
-        caller = "codespaces"
-    elif os.getenv("VSCODE_PID") or os.getenv("VSCODE_NLS_CONFIG"):
-        caller = "vscode"
-    elif os.getenv("GITPOD_WORKSPACE_ID") or os.getenv("GITPOD_WORKSPACE_URL"):
-        caller = "gitpod"
-    return app.set_session_var("caller_id", caller)
+        app.set_session_var("caller_id", caller)
 
 
 class Upgrader:
     def __init__(self, from_version, to_version):
         self.from_version = pepver_to_semver(from_version)
         self.to_version = pepver_to_semver(to_version)
 
         self._upgraders = [
-            (semantic_version.Version("3.5.0-a.2"), self._update_dev_platforms),
             (semantic_version.Version("4.4.0-a.8"), self._update_pkg_metadata),
         ]
 
     def run(self, ctx):
         if self.from_version > self.to_version:
             return True
 
@@ -97,19 +95,14 @@
             if self.from_version >= version or self.to_version < version:
                 continue
             result.append(callback(ctx))
 
         return all(result)
 
     @staticmethod
-    def _update_dev_platforms(ctx):
-        ctx.invoke(cmd_platform_update)
-        return True
-
-    @staticmethod
     def _update_pkg_metadata(_):
         pm = ToolPackageManager()
         for pkg in pm.get_installed():
             if not pkg.metadata or pkg.metadata.spec.external or pkg.metadata.spec.id:
                 continue
             result = pm.search_registry_packages(PackageSpec(name=pkg.metadata.name))
             if len(result) != 1:
@@ -162,16 +155,14 @@
                 fg="green",
             )
             telemetry.send_event(
                 category="Auto",
                 action="Upgrade",
                 label="%s > %s" % (last_version, __version__),
             )
-        else:
-            raise exception.UpgradeError("Auto upgrading...")
 
     # PlatformIO banner
     click.echo("*" * terminal_width)
     click.echo("If you like %s, please:" % (click.style("PlatformIO", fg="cyan")))
     click.echo(
         "- %s us on Twitter to stay up-to-date "
         "on the latest project news > %s"
```

### Comparing `platformio-6.1.6/platformio/package/__init__.py` & `platformio-6.1.7/platformio/package/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/cli.py` & `platformio-6.1.7/platformio/package/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/commands/__init__.py` & `platformio-6.1.7/platformio/package/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/commands/exec.py` & `platformio-6.1.7/platformio/package/commands/exec.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/commands/install.py` & `platformio-6.1.7/platformio/package/commands/install.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @click.command(
     "install", short_help="Install the project dependencies or custom packages"
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("-p", "--platform", "platforms", metavar="SPECIFICATION", multiple=True)
 @click.option("-t", "--tool", "tools", metavar="SPECIFICATION", multiple=True)
 @click.option("-l", "--library", "libraries", metavar="SPECIFICATION", multiple=True)
 @click.option(
     "--no-save",
@@ -51,15 +51,15 @@
     help="Prevent saving specified packages to `platformio.ini`",
 )
 @click.option("--skip-dependencies", is_flag=True, help="Skip package dependencies")
 @click.option("-g", "--global", is_flag=True, help="Install package globally")
 @click.option(
     "--storage-dir",
     default=None,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help="Custom Package Manager storage for global packages",
 )
 @click.option("-f", "--force", is_flag=True, help="Reinstall package if it exists")
 @click.option("-s", "--silent", is_flag=True, help="Suppress progress reporting")
 def package_install_cmd(**options):
     if options.get("global") or options.get("storage_dir"):
         install_global_dependencies(options)
```

### Comparing `platformio-6.1.6/platformio/package/commands/list.py` & `platformio-6.1.7/platformio/package/commands/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 
 
 @click.command("list", short_help="List installed packages")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("-p", "--platform", "platforms", metavar="SPECIFICATION", multiple=True)
 @click.option("-t", "--tool", "tools", metavar="SPECIFICATION", multiple=True)
 @click.option("-l", "--library", "libraries", metavar="SPECIFICATION", multiple=True)
 @click.option("-g", "--global", is_flag=True, help="List globally installed packages")
 @click.option(
     "--storage-dir",
     default=None,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help="Custom Package Manager storage for global packages",
 )
 @click.option("--only-platforms", is_flag=True, help="List only platform packages")
 @click.option("--only-tools", is_flag=True, help="List only tool packages")
 @click.option("--only-libraries", is_flag=True, help="List only library packages")
 @click.option("-v", "--verbose", is_flag=True)
 def package_list_cmd(**options):
@@ -133,15 +133,15 @@
         ("platforms", PlatformPackageManager(options.get("storage_dir"))),
         ("tools", ToolPackageManager(options.get("storage_dir"))),
         ("libraries", LibraryPackageManager(options.get("storage_dir"))),
     ]
     only_packages = any(
         options.get(type_) or options.get(f"only_{type_}") for (type_, _) in data
     )
-    for (type_, pm) in data:
+    for type_, pm in data:
         skip_conds = [
             only_packages
             and not options.get(type_)
             and not options.get(f"only_{type_}"),
             not pm.get_installed(),
         ]
         if any(skip_conds):
```

### Comparing `platformio-6.1.6/platformio/package/commands/outdated.py` & `platformio-6.1.7/platformio/package/commands/outdated.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 
 @click.command("outdated", short_help="Check for outdated packages")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 def package_outdated_cmd(project_dir, environments):
     candidates = fetch_outdated_candidates(
         project_dir, environments, with_progress=True
     )
     print_outdated_candidates(candidates)
```

### Comparing `platformio-6.1.6/platformio/package/commands/pack.py` & `platformio-6.1.7/platformio/package/commands/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 @click.command("pack", short_help="Create a tarball from a package")
 @click.argument(
     "package",
     default=os.getcwd,
     metavar="<source directory, tar.gz or zip>",
-    type=click.Path(exists=True, file_okay=True, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=True, dir_okay=True),
 )
 @click.option(
     "-o", "--output", help="A destination path (folder or a full path to file)"
 )
 def package_pack_cmd(package, output):
     p = PackagePacker(package)
     archive_path = p.pack(output)
```

### Comparing `platformio-6.1.6/platformio/package/commands/publish.py` & `platformio-6.1.7/platformio/package/commands/publish.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 @click.command("publish", short_help="Publish a package to the registry")
 @click.argument(
     "package",
     default=os.getcwd,
     metavar="<source directory, tar.gz or zip>",
-    type=click.Path(exists=True, file_okay=True, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=True, dir_okay=True),
 )
 @click.option(
     "--owner",
     help="PIO Account username (can be organization username). "
     "Default is set to a username of the authorized PIO Account",
 )
 @click.option(
```

### Comparing `platformio-6.1.6/platformio/package/commands/search.py` & `platformio-6.1.7/platformio/package/commands/search.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/commands/show.py` & `platformio-6.1.7/platformio/package/commands/show.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/commands/uninstall.py` & `platformio-6.1.7/platformio/package/commands/uninstall.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @click.command(
     "uninstall", short_help="Uninstall the project dependencies or custom packages"
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("-p", "--platform", "platforms", metavar="SPECIFICATION", multiple=True)
 @click.option("-t", "--tool", "tools", metavar="SPECIFICATION", multiple=True)
 @click.option("-l", "--library", "libraries", metavar="SPECIFICATION", multiple=True)
 @click.option(
     "--no-save",
@@ -45,15 +45,15 @@
     help="Prevent removing specified packages from `platformio.ini`",
 )
 @click.option("--skip-dependencies", is_flag=True, help="Skip package dependencies")
 @click.option("-g", "--global", is_flag=True, help="Uninstall global packages")
 @click.option(
     "--storage-dir",
     default=None,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help="Custom Package Manager storage for global packages",
 )
 @click.option("-s", "--silent", is_flag=True, help="Suppress progress reporting")
 def package_uninstall_cmd(**options):
     if options.get("global"):
         uninstall_global_dependencies(options)
     else:
```

### Comparing `platformio-6.1.6/platformio/package/commands/unpublish.py` & `platformio-6.1.7/platformio/package/commands/unpublish.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/commands/update.py` & `platformio-6.1.7/platformio/package/commands/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 @click.command(
     "update", short_help="Update the project dependencies or custom packages"
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("-p", "--platform", "platforms", metavar="SPECIFICATION", multiple=True)
 @click.option("-t", "--tool", "tools", metavar="SPECIFICATION", multiple=True)
 @click.option("-l", "--library", "libraries", metavar="SPECIFICATION", multiple=True)
 @click.option(
     "--no-save",
@@ -45,15 +45,15 @@
     help="Prevent saving specified packages to `platformio.ini`",
 )
 @click.option("--skip-dependencies", is_flag=True, help="Skip package dependencies")
 @click.option("-g", "--global", is_flag=True, help="Update global packages")
 @click.option(
     "--storage-dir",
     default=None,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
     help="Custom Package Manager storage for global packages",
 )
 @click.option("-s", "--silent", is_flag=True, help="Suppress progress reporting")
 def package_update_cmd(**options):
     if options.get("global"):
         update_global_dependencies(options)
     else:
```

### Comparing `platformio-6.1.6/platformio/package/download.py` & `platformio-6.1.7/platformio/package/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 else:
                     with click.progressbar(
                         length=file_size,
                         iterable=itercontent,
                         label=label,
                         update_min_steps=min(
                             256 * 1024, file_size / 100
-                        ),  # every 256Kb or less,
+                        ),  # every 256Kb or less
                     ) as pb:
                         for chunk in pb:
                             pb.update(len(chunk))
                             fp.write(chunk)
         finally:
             self._http_response.close()
             self._http_session.close()
```

### Comparing `platformio-6.1.6/platformio/package/exception.py` & `platformio-6.1.7/platformio/package/exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,28 +44,25 @@
             "Invalid manifest fields: %s. \nPlease check specification -> "
             "https://docs.platformio.org/page/librarymanager/config.html"
             % self.messages
         )
 
 
 class MissingPackageManifestError(ManifestException):
-
     MESSAGE = "Could not find one of '{0}' manifest files in the package"
 
 
 class UnknownPackageError(UserSideException):
-
     MESSAGE = (
         "Could not find the package with '{0}' requirements for your system '%s'"
         % util.get_systype()
     )
 
 
 class NotGlobalLibDir(UserSideException):
-
     MESSAGE = (
         "The `{0}` is not a PlatformIO project.\n\n"
         "To manage libraries in global storage `{1}`,\n"
         "please use `platformio lib --global {2}` or specify custom storage "
         "`platformio lib --storage-dir /path/to/storage/ {2}`.\n"
         "Check `platformio lib --help` for details."
     )
```

### Comparing `platformio-6.1.6/platformio/package/lockfile.py` & `platformio-6.1.7/platformio/package/lockfile.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/__init__.py` & `platformio-6.1.7/platformio/package/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/_download.py` & `platformio-6.1.7/platformio/package/manager/_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from platformio import app, compat, util
 from platformio.package.download import FileDownloader
 from platformio.package.lockfile import LockFile
 
 
 class PackageManagerDownloadMixin:
-
     DOWNLOAD_CACHE_EXPIRE = 86400 * 30  # keep package in a local cache for 1 month
 
     def compute_download_path(self, *args):
         request_hash = hashlib.new("sha1")
         for arg in args:
             request_hash.update(compat.hashlib_encode_data(arg))
         dl_path = os.path.join(self.get_download_dir(), request_hash.hexdigest())
@@ -58,24 +57,24 @@
     def download(self, url, checksum=None):
         silent = not self.log.isEnabledFor(logging.INFO)
         dl_path = self.compute_download_path(url, checksum or "")
         if os.path.isfile(dl_path):
             self.set_download_utime(dl_path)
             return dl_path
 
-        with_progress = not silent and not app.is_disabled_progressbar()
+        with_progress = not app.is_disabled_progressbar()
         tmp_fd, tmp_path = tempfile.mkstemp(dir=self.get_download_dir())
         try:
             with LockFile(dl_path):
                 try:
                     fd = FileDownloader(url)
                     fd.set_destination(tmp_path)
                     fd.start(with_progress=with_progress, silent=silent)
                 except IOError as exc:
-                    raise_error = not with_progress
+                    raise_error = not silent
                     if with_progress:
                         try:
                             fd = FileDownloader(url)
                             fd.set_destination(tmp_path)
                             fd.start(with_progress=False, silent=silent)
                         except IOError:
                             raise_error = True
```

### Comparing `platformio-6.1.6/platformio/package/manager/_install.py` & `platformio-6.1.7/platformio/package/manager/_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 from platformio.package.exception import PackageException, UnknownPackageError
 from platformio.package.meta import PackageCompatibility, PackageItem
 from platformio.package.unpack import FileUnpacker
 from platformio.package.vcsclient import VCSClientFactory
 
 
 class PackageManagerInstallMixin:
-
     _INSTALL_HISTORY = None  # avoid circle dependencies
 
     @staticmethod
     def unpack(src, dst):
         with_progress = not app.is_disabled_progressbar()
         try:
             with FileUnpacker(src) as fu:
```

### Comparing `platformio-6.1.6/platformio/package/manager/_legacy.py` & `platformio-6.1.7/platformio/package/manager/_legacy.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/_registry.py` & `platformio-6.1.7/platformio/package/manager/_registry.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/_symlink.py` & `platformio-6.1.7/platformio/package/manager/_symlink.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/_uninstall.py` & `platformio-6.1.7/platformio/package/manager/_uninstall.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/_update.py` & `platformio-6.1.7/platformio/package/manager/_update.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/base.py` & `platformio-6.1.7/platformio/package/manager/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/library.py` & `platformio-6.1.7/platformio/package/manager/library.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manager/platform.py` & `platformio-6.1.7/platformio/package/manager/platform.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 
 from platformio import util
-from platformio.http import HTTPClientError, InternetIsOffline
+from platformio.http import HTTPClientError, InternetConnectionError
 from platformio.package.exception import UnknownPackageError
 from platformio.package.manager.base import BasePackageManager
 from platformio.package.manager.core import get_installed_core_packages
 from platformio.package.manager.tool import ToolPackageManager
 from platformio.package.meta import PackageType
 from platformio.platform.exception import IncompatiblePlatform, UnknownBoard
 from platformio.platform.factory import PlatformFactory
@@ -124,15 +124,15 @@
         boards = self.get_installed_boards()
         know_boards = ["%s:%s" % (b["platform"], b["id"]) for b in boards]
         try:
             for board in self.get_registered_boards():
                 key = "%s:%s" % (board["platform"], board["id"])
                 if key not in know_boards:
                     boards.append(board)
-        except (HTTPClientError, InternetIsOffline):
+        except (HTTPClientError, InternetConnectionError):
             pass
         return sorted(boards, key=lambda b: b["name"])
 
     def board_config(self, id_, platform=None):
         for manifest in self.get_installed_boards():
             if manifest["id"] == id_ and (
                 not platform or manifest["platform"] == platform
```

### Comparing `platformio-6.1.6/platformio/package/manager/tool.py` & `platformio-6.1.7/platformio/package/manager/tool.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manifest/__init__.py` & `platformio-6.1.7/platformio/package/manifest/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manifest/parser.py` & `platformio-6.1.7/platformio/package/manifest/parser.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/manifest/schema.py` & `platformio-6.1.7/platformio/package/manifest/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,13 +272,13 @@
             "Invalid SPDX license identifier. See valid identifiers at "
             "https://spdx.org/licenses/"
         )
 
     @staticmethod
     @memoized(expire="1h")
     def load_spdx_licenses():
-        version = "3.19"
+        version = "3.20"
         spdx_data_url = (
             "https://raw.githubusercontent.com/spdx/license-list-data/"
             "v%s/json/licenses.json" % version
         )
         return json.loads(fetch_remote_content(spdx_data_url))
```

### Comparing `platformio-6.1.6/platformio/package/meta.py` & `platformio-6.1.7/platformio/package/meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
                             return t
                     except KeyError:
                         pass
         return None
 
 
 class PackageCompatibility:
-
     KNOWN_QUALIFIERS = ("platforms", "frameworks", "authors")
 
     @classmethod
     def from_dependency(cls, dependency):
         assert isinstance(dependency, dict)
         qualifiers = {
             key: value
@@ -464,15 +463,14 @@
                 data["spec"]["uri"] = data["spec"]["url"]
                 del data["spec"]["url"]
             data["spec"] = PackageSpec(**data["spec"])
         return PackageMetaData(**data)
 
 
 class PackageItem:
-
     METAFILE_NAME = ".piopm"
 
     def __init__(self, path, metadata=None):
         self.path = path
         self.metadata = metadata
         if not self.metadata and self.exists():
             self.metadata = self.load_meta()
```

### Comparing `platformio-6.1.6/platformio/package/pack.py` & `platformio-6.1.7/platformio/package/pack.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/package/unpack.py` & `platformio-6.1.7/platformio/package/unpack.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from tarfile import open as tarfile_open
 from time import mktime
 from zipfile import ZipFile
 
 import click
 
 from platformio import fs
+from platformio.compat import is_terminal
 from platformio.package.exception import PackageException
 
 
 class ExtractArchiveItemError(PackageException):
-
     MESSAGE = (
         "Could not extract `{0}` to `{1}`. Try to disable antivirus "
         "tool or check this solution -> https://bit.ly/faq-package-manager"
     )
 
 
 class BaseArchiver:
@@ -155,26 +155,46 @@
             for magic, archiver in magic_map.items():
                 if data.startswith(magic):
                     return archiver(path)
         raise PackageException("Unknown archive type '%s'" % path)
 
     def unpack(
         self, dest_dir=None, with_progress=True, check_unpacked=True, silent=False
-    ):
+    ):  # pylint: disable=too-many-branches
         assert self._archiver
+        label = "Unpacking"
+        items = self._archiver.get_items()
         if not dest_dir:
             dest_dir = os.getcwd()
+
         if not with_progress or silent:
             if not silent:
-                click.echo("Unpacking...")
-            for item in self._archiver.get_items():
+                click.echo(f"{label}...")
+            for item in items:
+                self._archiver.extract_item(item, dest_dir)
+        elif not is_terminal():
+            click.echo(f"{label} 0%", nl=False)
+            print_percent_step = 10
+            printed_percents = 0
+            unpacked_nums = 0
+            for item in items:
                 self._archiver.extract_item(item, dest_dir)
+                unpacked_nums += 1
+                if (unpacked_nums / len(items) * 100) >= (
+                    printed_percents + print_percent_step
+                ):
+                    printed_percents += print_percent_step
+                    click.echo(f" {printed_percents}%", nl=False)
+            click.echo("")
         else:
-            items = self._archiver.get_items()
-            with click.progressbar(items, label="Unpacking") as pb:
+            with click.progressbar(
+                items,
+                label=label,
+                update_min_steps=min(50, len(items) / 100),  # every 50 files or less
+            ) as pb:
                 for item in pb:
                     self._archiver.extract_item(item, dest_dir)
 
         if not check_unpacked:
             return True
 
         # check on disk
```

### Comparing `platformio-6.1.6/platformio/package/vcsclient.py` & `platformio-6.1.7/platformio/package/vcsclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,14 @@
         except (KeyError, AssertionError) as exc:
             raise VCSBaseException(
                 "VCS: Unknown repository type %s" % remote_url
             ) from exc
 
 
 class VCSClientBase:
-
     command = None
 
     def __init__(self, src_dir, remote_url=None, tag=None, silent=False):
         self.src_dir = src_dir
         self.remote_url = remote_url
         self.tag = tag
         self.silent = silent
@@ -124,15 +123,14 @@
             return result["out"].strip()
         raise VCSBaseException(
             "VCS: Could not receive an output from `%s` command (%s)" % (args, result)
         )
 
 
 class GitClient(VCSClientBase):
-
     command = "git"
     _configured = False
 
     def __init__(self, *args, **kwargs):
         self.configure()
         super().__init__(*args, **kwargs)
 
@@ -228,15 +226,14 @@
             if ref == branch_ref:
                 return sha[:7]
 
         return None
 
 
 class HgClient(VCSClientBase):
-
     command = "hg"
 
     def export(self):
         args = ["clone"]
         if self.tag:
             args.extend(["--updaterev", self.tag])
         args.extend([self.remote_url, self.src_dir])
@@ -252,15 +249,14 @@
     def get_latest_revision(self):
         if not self.can_be_updated:
             return self.get_latest_revision()
         return self.get_cmd_output(["identify", "--id", self.remote_url])
 
 
 class SvnClient(VCSClientBase):
-
     command = "svn"
 
     def export(self):
         args = ["checkout"]
         if self.tag:
             args.extend(["--revision", self.tag])
         args.extend([self.remote_url, self.src_dir])
```

### Comparing `platformio-6.1.6/platformio/package/version.py` & `platformio-6.1.7/platformio/package/version.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/platform/__init__.py` & `platformio-6.1.7/platformio/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/platform/_packages.py` & `platformio-6.1.7/platformio/platform/_packages.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/platform/_run.py` & `platformio-6.1.7/platformio/platform/_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 
 import click
 
 from platformio import app, fs, proc, telemetry
 from platformio.compat import hashlib_encode_data
 from platformio.package.manager.core import get_core_package_dir
 from platformio.platform.exception import BuildScriptNotFound
+from platformio.run.helpers import KNOWN_CLEAN_TARGETS, KNOWN_FULLCLEAN_TARGETS
 
 
 class PlatformRunMixin:
-
     LINE_ERROR_RE = re.compile(r"(^|\s+)error:?\s+", re.I)
 
     @staticmethod
     def encode_scons_arg(value):
         if isinstance(value, (list, tuple, dict)):
             value = json.dumps(value)
         return base64.urlsafe_b64encode(hashlib_encode_data(value)).decode()
@@ -53,17 +53,14 @@
         self.ensure_engine_compatible()
         self.configure_project_packages(variables["pioenv"], targets)
         self._report_non_sensitive_data(variables["pioenv"], targets)
 
         self.silent = silent
         self.verbose = verbose or app.get_setting("force_verbose")
 
-        if "clean" in targets:
-            targets = ["-c", "."]
-
         variables["platform_manifest"] = self.manifest_path
 
         if "build_script" not in variables:
             variables["build_script"] = self.get_build_script()
         if not os.path.isfile(variables["build_script"]):
             raise BuildScriptNotFound(variables["build_script"])
 
@@ -89,24 +86,30 @@
             "-Q",
             "--warn=no-no-parallel-support",
             "--jobs",
             str(jobs),
             "--sconstruct",
             os.path.join(fs.get_source_dir(), "builder", "main.py"),
         ]
-        args.append("PIOVERBOSE=%d" % (1 if self.verbose else 0))
+        args.append("PIOVERBOSE=%d" % int(self.verbose))
         # pylint: disable=protected-access
-        args.append("ISATTY=%d" % (1 if click._compat.isatty(sys.stdout) else 0))
-        args += targets
-
+        args.append("ISATTY=%d" % int(click._compat.isatty(sys.stdout)))
         # encode and append variables
         for key, value in variables.items():
             args.append("%s=%s" % (key.upper(), self.encode_scons_arg(value)))
 
-        proc.copy_pythonpath_to_osenv()
+        if set(KNOWN_CLEAN_TARGETS + KNOWN_FULLCLEAN_TARGETS) & set(targets):
+            args.append("--clean")
+            args.append(
+                "FULLCLEAN=%d"
+                % (1 if set(KNOWN_FULLCLEAN_TARGETS) & set(targets) else 0)
+            )
+        elif targets:
+            args.extend(targets)
+
         # force SCons output to Unicode
         os.environ["PYTHONIOENCODING"] = "utf-8"
 
         if targets and "menuconfig" in targets:
             return proc.exec_command(
                 args, stdout=sys.stdout, stderr=sys.stderr, stdin=sys.stdin
             )
```

### Comparing `platformio-6.1.6/platformio/platform/base.py` & `platformio-6.1.7/platformio/platform/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from platformio.platform.exception import IncompatiblePlatform, UnknownBoard
 from platformio.project.config import ProjectConfig
 
 
 class PlatformBase(  # pylint: disable=too-many-instance-attributes,too-many-public-methods
     PlatformPackagesMixin, PlatformRunMixin
 ):
-
     CORE_SEMVER = pepver_to_semver(__version__)
     _BOARDS_CACHE = {}
 
     def __init__(self, manifest_path):
         self.manifest_path = manifest_path
         self.silent = False
         self.verbose = False
@@ -204,14 +203,23 @@
                 # allow only upload tools and frameworks
                 elif "nobuild" in targets and opts.get("type") != "framework":
                     self.packages[name]["optional"] = True
 
     def configure_debug_session(self, debug_config):
         raise NotImplementedError
 
+    def generate_sample_code(self, project_config, environment):
+        raise NotImplementedError
+
+    def on_installed(self):
+        pass
+
+    def on_uninstalled(self):
+        pass
+
     def get_lib_storages(self):
         storages = {}
         for opts in (self.frameworks or {}).values():
             if "package" not in opts:
                 continue
             pkg = self.get_package(opts["package"])
             if not pkg or not os.path.isdir(os.path.join(pkg.path, "libraries")):
@@ -224,13 +232,7 @@
             for item in os.listdir(libcores_dir):
                 libcore_dir = os.path.join(libcores_dir, item)
                 if not os.path.isdir(libcore_dir):
                     continue
                 storages[libcore_dir] = "%s-core-%s" % (opts["package"], item)
 
         return [dict(name=name, path=path) for path, name in storages.items()]
-
-    def on_installed(self):
-        pass
-
-    def on_uninstalled(self):
-        pass
```

### Comparing `platformio-6.1.6/platformio/platform/board.py` & `platformio-6.1.7/platformio/platform/board.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/platform/exception.py` & `platformio-6.1.7/platformio/platform/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,31 @@
 
 
 class PlatformException(PlatformioException):
     pass
 
 
 class UnknownPlatform(PlatformException):
-
     MESSAGE = "Unknown development platform '{0}'"
 
 
 class IncompatiblePlatform(PlatformException):
-
     MESSAGE = (
         "Development platform '{0}' is not compatible with PlatformIO Core v{1} and "
         "depends on PlatformIO Core {2}.\n"
     )
 
 
 class UnknownBoard(PlatformException):
-
     MESSAGE = "Unknown board ID '{0}'"
 
 
 class InvalidBoardManifest(PlatformException):
-
     MESSAGE = "Invalid board JSON manifest '{0}'"
 
 
 class UnknownFramework(PlatformException):
-
     MESSAGE = "Unknown framework '{0}'"
 
 
 class BuildScriptNotFound(PlatformException):
-
     MESSAGE = "Invalid path '{0}' to build script"
```

### Comparing `platformio-6.1.6/platformio/platform/factory.py` & `platformio-6.1.7/platformio/platform/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/proc.py` & `platformio-6.1.7/platformio/proc.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/project/__init__.py` & `platformio-6.1.7/platformio/project/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/project/cli.py` & `platformio-6.1.7/platformio/project/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/project/commands/__init__.py` & `platformio-6.1.7/platformio/project/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/project/commands/config.py` & `platformio-6.1.7/platformio/project/commands/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 
 @click.command("config", short_help="Show computed configuration")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("--json-output", is_flag=True)
 def project_config_cmd(project_dir, json_output):
     if not is_platformio_project(project_dir):
         raise NotPlatformIOProjectError(project_dir)
     with fs.cd(project_dir):
         config = ProjectConfig.get_instance()
```

### Comparing `platformio-6.1.6/platformio/project/commands/init.py` & `platformio-6.1.7/platformio/project/commands/init.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 
 import click
 
 from platformio import fs
 from platformio.package.commands.install import install_project_dependencies
 from platformio.package.manager.platform import PlatformPackageManager
 from platformio.platform.exception import UnknownBoard
+from platformio.platform.factory import PlatformFactory
 from platformio.project.config import ProjectConfig
 from platformio.project.helpers import is_platformio_project
 from platformio.project.integration.generator import ProjectGenerator
+from platformio.project.options import ProjectOptions
 
 
-def validate_boards(ctx, param, value):  # pylint: disable=W0613
+def validate_boards(ctx, param, value):  # pylint: disable=unused-argument
     pm = PlatformPackageManager()
     for id_ in value:
         try:
             pm.board_config(id_)
         except UnknownBoard as exc:
             raise click.BadParameter(
                 "`%s`. Please search for board ID using `platformio boards` "
@@ -43,134 +45,127 @@
 
 
 @click.command("init", short_help="Initialize a project or update existing")
 @click.option(
     "--project-dir",
     "-d",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
+)
+@click.option(
+    "-b", "--board", "boards", multiple=True, metavar="ID", callback=validate_boards
 )
-@click.option("-b", "--board", multiple=True, metavar="ID", callback=validate_boards)
 @click.option("--ide", type=click.Choice(ProjectGenerator.get_supported_ides()))
 @click.option("-e", "--environment", help="Update existing environment")
-@click.option("-O", "--project-option", multiple=True)
-@click.option("--env-prefix", default="")
+@click.option(
+    "-O",
+    "--project-option",
+    "project_options",
+    multiple=True,
+    help="A `name=value` pair",
+)
+@click.option("--sample-code", is_flag=True)
 @click.option("--no-install-dependencies", is_flag=True)
+@click.option("--env-prefix", default="")
 @click.option("-s", "--silent", is_flag=True)
 def project_init_cmd(
     project_dir,
-    board,
+    boards,
     ide,
     environment,
-    project_option,
-    env_prefix,
+    project_options,
+    sample_code,
     no_install_dependencies,
+    env_prefix,
     silent,
 ):
     is_new_project = not is_platformio_project(project_dir)
     if is_new_project:
         if not silent:
             print_header(project_dir)
         init_base_project(project_dir)
 
-    if environment:
-        update_project_env(project_dir, environment, project_option)
-    elif board:
-        update_board_envs(project_dir, board, project_option, env_prefix)
-
     with fs.cd(project_dir):
+        if environment:
+            update_project_env(environment, project_options)
+        elif boards:
+            update_board_envs(project_dir, boards, project_options, env_prefix)
+
         generator = None
         config = ProjectConfig.get_instance(os.path.join(project_dir, "platformio.ini"))
         if ide:
             config.validate()
             # init generator and pick the best env if user didn't specify
-            generator = ProjectGenerator(config, environment, ide, board)
+            generator = ProjectGenerator(config, environment, ide, boards)
             if not environment:
                 environment = generator.env_name
 
         # resolve project dependencies
-        if not no_install_dependencies and (environment or board):
+        if not no_install_dependencies and (environment or boards):
             install_project_dependencies(
                 options=dict(
                     project_dir=project_dir,
                     environments=[environment] if environment else [],
                     silent=silent,
                 )
             )
 
+        if environment and sample_code:
+            init_sample_code(config, environment)
+
         if generator:
             if not silent:
                 click.echo(
                     "Updating metadata for the %s IDE..." % click.style(ide, fg="cyan")
                 )
             generator.generate()
 
-    if is_new_project:
-        init_cvs_ignore(project_dir)
+        if is_new_project:
+            init_cvs_ignore()
 
     if not silent:
         print_footer(is_new_project)
 
 
 def print_header(project_dir):
-    if project_dir == os.getcwd():
-        click.secho("\nThe current working directory ", fg="yellow", nl=False)
-        try:
-            click.secho(project_dir, fg="cyan", nl=False)
-        except UnicodeEncodeError:
-            click.secho(json.dumps(project_dir), fg="cyan", nl=False)
-        click.secho(" will be used for the project.", fg="yellow")
-        click.echo("")
-
-    click.echo("The next files/directories have been created in ", nl=False)
+    click.echo("The following files/directories have been created in ", nl=False)
     try:
         click.secho(project_dir, fg="cyan")
     except UnicodeEncodeError:
         click.secho(json.dumps(project_dir), fg="cyan")
     click.echo("%s - Put project header files here" % click.style("include", fg="cyan"))
     click.echo(
-        "%s - Put here project specific (private) libraries"
+        "%s - Put project specific (private) libraries here"
         % click.style("lib", fg="cyan")
     )
     click.echo("%s - Put project source files here" % click.style("src", fg="cyan"))
     click.echo(
         "%s - Project Configuration File" % click.style("platformio.ini", fg="cyan")
     )
 
 
 def print_footer(is_new_project):
-    if is_new_project:
-        return click.secho(
-            "\nProject has been successfully initialized! Useful commands:\n"
-            "`pio run` - process/build project from the current directory\n"
-            "`pio run --target upload` or `pio run -t upload` "
-            "- upload firmware to a target\n"
-            "`pio run --target clean` - clean project (remove compiled files)"
-            "\n`pio run --help` - additional information",
-            fg="green",
-        )
+    action = "initialized" if is_new_project else "updated"
     return click.secho(
-        "Project has been successfully updated!",
+        f"Project has been successfully {action}!",
         fg="green",
     )
 
 
 def init_base_project(project_dir):
     with fs.cd(project_dir):
         config = ProjectConfig()
         config.save()
         dir_to_readme = [
             (config.get("platformio", "src_dir"), None),
             (config.get("platformio", "include_dir"), init_include_readme),
             (config.get("platformio", "lib_dir"), init_lib_readme),
             (config.get("platformio", "test_dir"), init_test_readme),
         ]
-        for (path, cb) in dir_to_readme:
+        for path, cb in dir_to_readme:
             if os.path.isdir(path):
                 continue
             os.makedirs(path)
             if cb:
                 cb(path)
 
 
@@ -287,48 +282,48 @@
 
 More information about PlatformIO Unit Testing:
 - https://docs.platformio.org/en/latest/advanced/unit-testing/index.html
 """,
         )
 
 
-def init_cvs_ignore(project_dir):
-    conf_path = os.path.join(project_dir, ".gitignore")
+def init_cvs_ignore():
+    conf_path = ".gitignore"
     if os.path.isfile(conf_path):
         return
     with open(conf_path, mode="w", encoding="utf8") as fp:
         fp.write(".pio\n")
 
 
-def update_board_envs(project_dir, board_ids, project_option, env_prefix):
+def update_board_envs(project_dir, boards, extra_project_options, env_prefix):
     config = ProjectConfig(
         os.path.join(project_dir, "platformio.ini"), parse_extra=False
     )
     used_boards = []
     for section in config.sections():
         cond = [section.startswith("env:"), config.has_option(section, "board")]
         if all(cond):
             used_boards.append(config.get(section, "board"))
 
     pm = PlatformPackageManager()
     modified = False
-    for id_ in board_ids:
+    for id_ in boards:
         board_config = pm.board_config(id_)
         if id_ in used_boards:
             continue
         used_boards.append(id_)
         modified = True
 
         envopts = {"platform": board_config["platform"], "board": id_}
         # find default framework for board
         frameworks = board_config.get("frameworks")
         if frameworks:
             envopts["framework"] = frameworks[0]
 
-        for item in project_option:
+        for item in extra_project_options:
             if "=" not in item:
                 continue
             _name, _value = item.split("=", 1)
             envopts[_name.strip()] = _value.strip()
 
         section = "env:%s%s" % (env_prefix, id_)
         config.add_section(section)
@@ -336,25 +331,80 @@
         for option, value in envopts.items():
             config.set(section, option, value)
 
     if modified:
         config.save()
 
 
-def update_project_env(project_dir, environment, project_option):
-    if not project_option:
+def update_project_env(environment, extra_project_options=None):
+    if not extra_project_options:
         return
+    env_section = "env:%s" % environment
+    option_to_sections = {"platformio": [], env_section: []}
+    for item in extra_project_options:
+        assert "=" in item
+        name, value = item.split("=", 1)
+        name = name.strip()
+        destination = env_section
+        for option in ProjectOptions.values():
+            if option.scope in option_to_sections and option.name == name:
+                destination = option.scope
+                break
+        option_to_sections[destination].append((name, value.strip()))
+
     config = ProjectConfig(
-        os.path.join(project_dir, "platformio.ini"), parse_extra=False
+        "platformio.ini", parse_extra=False, expand_interpolations=False
     )
-
-    section = "env:%s" % environment
-    if not config.has_section(section):
-        config.add_section(section)
-
-    for item in project_option:
-        if "=" not in item:
+    for section, options in option_to_sections.items():
+        if not options:
             continue
-        _name, _value = item.split("=", 1)
-        config.set(section, _name.strip(), _value.strip())
+        if not config.has_section(section):
+            config.add_section(section)
+        for name, value in options:
+            config.set(section, name, value)
 
     config.save()
+
+
+def init_sample_code(config, environment):
+    platform_spec = config.get(f"env:{environment}", "platform", None)
+    if not platform_spec:
+        return None
+    p = PlatformFactory.new(platform_spec)
+    try:
+        return p.generate_sample_code(config, environment)
+    except NotImplementedError:
+        pass
+
+    framework = config.get(f"env:{environment}", "framework", None)
+    if framework != ["arduino"]:
+        return None
+    main_content = """
+#include <Arduino.h>
+
+// put function declarations here:
+int myFunction(int, int);
+
+void setup() {
+  // put your setup code here, to run once:
+  int result = myFunction(2, 3);
+}
+
+void loop() {
+  // put your main code here, to run repeatedly:
+}
+
+// put function definitions here:
+int myFunction(int x, int y) {
+  return x + y;
+}
+"""
+    is_cpp_project = p.name not in ["intel_mcs51", "ststm8"]
+    src_dir = config.get("platformio", "src_dir")
+    main_path = os.path.join(src_dir, "main.%s" % ("cpp" if is_cpp_project else "c"))
+    if os.path.isfile(main_path):
+        return None
+    if not os.path.isdir(src_dir):
+        os.makedirs(src_dir)
+    with open(main_path, mode="w", encoding="utf8") as fp:
+        fp.write(main_content.strip())
+    return True
```

### Comparing `platformio-6.1.6/platformio/project/commands/metadata.py` & `platformio-6.1.7/platformio/project/commands/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 @click.command(
     "metadata", short_help="Dump metadata intended for IDE extensions/plugins"
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option("-e", "--environment", "environments", multiple=True)
 @click.option("--json-output", is_flag=True)
-@click.option("--json-output-path", type=click.Path(resolve_path=True))
+@click.option("--json-output-path", type=click.Path())
 def project_metadata_cmd(project_dir, environments, json_output, json_output_path):
     with fs.cd(project_dir):
         config = ProjectConfig.get_instance()
         config.validate(environments)
         environments = list(environments or config.envs())
         build_metadata = load_build_metadata(project_dir, environments)
```

### Comparing `platformio-6.1.6/platformio/project/config.py` & `platformio-6.1.7/platformio/project/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ;
 ; Please visit documentation for the other options and examples
 ; https://docs.platformio.org/page/projectconf.html
 """
 
 
 class ProjectConfigBase:
-
+    ENVNAME_RE = re.compile(r"^[a-z\d\_\-]+$", flags=re.I)
     INLINE_COMMENT_RE = re.compile(r"\s+;.*$")
     VARTPL_RE = re.compile(r"\$\{([^\.\}\()]+)\.([^\}]+)\}")
 
     CUSTOM_OPTION_PREFIXES = ("custom_", "board_")
 
     expand_interpolations = True
     warnings = []
@@ -385,38 +385,59 @@
             return default_envs[0]
         envs = self.envs()
         return envs[0] if envs else None
 
     def validate(self, envs=None, silent=False):
         if not os.path.isfile(self.path):
             raise exception.NotPlatformIOProjectError(os.path.dirname(self.path))
+
+        known_envs = set(self.envs())
+
         # check envs
-        known = set(self.envs())
-        if not known:
+        if not known_envs:
             raise exception.ProjectEnvsNotAvailableError()
-        unknown = set(list(envs or []) + self.default_envs()) - known
-        if unknown:
-            raise exception.UnknownEnvNamesError(", ".join(unknown), ", ".join(known))
+        unknown_envs = set(list(envs or []) + self.default_envs()) - known_envs
+        if unknown_envs:
+            raise exception.UnknownEnvNamesError(
+                ", ".join(unknown_envs), ", ".join(known_envs)
+            )
+
+        for env in known_envs:
+            # check envs names
+            if not self.ENVNAME_RE.match(env):
+                raise exception.InvalidEnvNameError(env)
+
+            # check simultaneous use of `monitor_raw` and `monitor_filters`
+            if self.get(f"env:{env}", "monitor_raw", False) and self.get(
+                f"env:{env}", "monitor_filters", None
+            ):
+                self.warnings.append(
+                    "The `monitor_raw` and `monitor_filters` options cannot be "
+                    f"used simultaneously for the `{env}` environment in the "
+                    "`platformio.ini` file. The `monitor_filters` option will "
+                    "be disabled to avoid conflicts."
+                )
+
         if not silent:
             for warning in self.warnings:
                 click.secho("Warning! %s" % warning, fg="yellow")
+
         return True
 
 
 class ProjectConfigDirsMixin:
     def get_optional_dir(self, name):
         """
         Deprecated, used by platformio-node-helpers.project.observer.fetchLibDirs
         PlatformIO IDE for Atom depends on platformio-node-helpers@~7.2.0
         """
         return self.get("platformio", f"{name}_dir")
 
 
 class ProjectConfig(ProjectConfigBase, ProjectConfigDirsMixin):
-
     _instances = {}
 
     @staticmethod
     def get_instance(path=None):
         path = ProjectConfig.get_default_path() if path is None else path
         mtime = os.path.getmtime(path) if os.path.isfile(path) else 0
         instance = ProjectConfig._instances.get(path)
```

### Comparing `platformio-6.1.6/platformio/project/exception.py` & `platformio-6.1.7/platformio/project/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,38 +16,39 @@
 
 
 class ProjectError(PlatformioException):
     pass
 
 
 class NotPlatformIOProjectError(ProjectError, UserSideException):
-
     MESSAGE = (
         "Not a PlatformIO project. `platformio.ini` file has not been "
         "found in current working directory ({0}). To initialize new project "
         "please use `platformio project init` command"
     )
 
 
 class InvalidProjectConfError(ProjectError, UserSideException):
-
     MESSAGE = "Invalid '{0}' (project configuration file): '{1}'"
 
 
 class UndefinedEnvPlatformError(ProjectError, UserSideException):
-
     MESSAGE = "Please specify platform for '{0}' environment"
 
 
 class ProjectEnvsNotAvailableError(ProjectError, UserSideException):
-
     MESSAGE = "Please setup environments in `platformio.ini` file"
 
 
 class UnknownEnvNamesError(ProjectError, UserSideException):
-
     MESSAGE = "Unknown environment names '{0}'. Valid names are '{1}'"
 
 
-class ProjectOptionValueError(ProjectError, UserSideException):
+class InvalidEnvNameError(ProjectError, UserSideException):
+    MESSAGE = (
+        "Invalid environment name '{0}'. The name can contain "
+        "alphanumeric, underscore, and hyphen characters (a-z, 0-9, -, _)"
+    )
 
+
+class ProjectOptionValueError(ProjectError, UserSideException):
     MESSAGE = "{0} for option `{1}` in section [{2}]"
```

### Comparing `platformio-6.1.6/platformio/project/helpers.py` & `platformio-6.1.7/platformio/project/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
+import re
 import subprocess
 from hashlib import sha1
 
 from click.testing import CliRunner
 
 from platformio import __version__, exception, fs
 from platformio.compat import IS_MACOS, IS_WINDOWS, hashlib_encode_data
 from platformio.project.config import ProjectConfig
 
 
 def get_project_dir():
-    return fs.normalize_path(os.getcwd())
+    return os.getcwd()
 
 
 def is_platformio_project(project_dir=None):
     if not project_dir:
         project_dir = get_project_dir()
     return os.path.isfile(os.path.join(project_dir, "platformio.ini"))
 
@@ -90,15 +91,24 @@
 
 
 def compute_project_checksum(config):
     # rebuild when PIO Core version changes
     checksum = sha1(hashlib_encode_data(__version__))
 
     # configuration file state
-    checksum.update(hashlib_encode_data(config.to_json()))
+    config_data = config.to_json()
+    if IS_WINDOWS:
+        # issue #4600: fix drive letter
+        config_data = re.sub(
+            r"([A-Z]):\\",
+            lambda match: "%s:\\" % match.group(1).lower(),
+            config_data,
+            flags=re.I,
+        )
+    checksum.update(hashlib_encode_data(config_data))
 
     # project file structure
     check_suffixes = (".c", ".cc", ".cpp", ".h", ".hpp", ".s", ".S")
     for d in (
         config.get("platformio", "include_dir"),
         config.get("platformio", "src_dir"),
         config.get("platformio", "lib_dir"),
```

### Comparing `platformio-6.1.6/platformio/project/integration/__init__.py` & `platformio-6.1.7/platformio/project/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/project/integration/generator.py` & `platformio-6.1.7/platformio/project/integration/generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,41 +15,42 @@
 import codecs
 import os
 import sys
 
 import bottle
 
 from platformio import fs, util
+from platformio.debug.helpers import get_default_debug_env
 from platformio.proc import where_is_program
 from platformio.project.helpers import load_build_metadata
 
 
 class ProjectGenerator:
-    def __init__(self, config, env_name, ide, board_ids=None):
+    def __init__(self, config, env_name, ide, boards=None):
         self.config = config
         self.project_dir = os.path.dirname(config.path)
-        self.original_env_name = env_name
-        self.env_name = str(env_name or self.get_best_envname(board_ids))
+        self.forced_env_name = env_name
+        self.env_name = str(env_name or self.get_best_envname(boards))
         self.ide = str(ide)
 
-    def get_best_envname(self, board_ids=None):
+    def get_best_envname(self, boards=None):
         envname = None
         default_envs = self.config.default_envs()
         if default_envs:
             envname = default_envs[0]
-            if not board_ids:
+            if not boards:
                 return envname
 
         for env in self.config.envs():
-            if not board_ids:
+            if not boards:
                 return env
             if not envname:
                 envname = env
             items = self.config.items(env=env, as_dict=True)
-            if "board" in items and items.get("board") in board_ids:
+            if "board" in items and items.get("board") in boards:
                 return env
         return envname
 
     @staticmethod
     def get_ide_tpls_dir():
         return os.path.join(fs.get_assets_dir(), "templates", "ide-projects")
 
@@ -82,15 +83,16 @@
         tpl_vars = {
             "config": self.config,
             "systype": util.get_systype(),
             "project_name": self.config.get(
                 "platformio", "name", os.path.basename(self.project_dir)
             ),
             "project_dir": self.project_dir,
-            "original_env_name": self.original_env_name,
+            "forced_env_name": self.forced_env_name,
+            "default_debug_env_name": get_default_debug_env(self.config),
             "env_name": self.env_name,
             "user_home_dir": os.path.abspath(fs.expanduser("~")),
             "platformio_path": sys.argv[0]
             if os.path.isfile(sys.argv[0])
             else where_is_program("platformio"),
             "env_path": os.getenv("PATH"),
             "env_pathsep": os.pathsep,
@@ -128,15 +130,15 @@
 
     def get_src_files(self):
         result = []
         with fs.cd(self.project_dir):
             for root, _, files in os.walk(self.config.get("platformio", "src_dir")):
                 for f in files:
                     result.append(
-                        os.path.relpath(os.path.join(os.path.realpath(root), f))
+                        os.path.relpath(os.path.join(os.path.abspath(root), f))
                     )
         return result
 
     def get_tpls(self):
         tpls = []
         ide_tpls_dir = os.path.join(self.get_ide_tpls_dir(), self.ide)
         for root, _, files in os.walk(ide_tpls_dir):
```

### Comparing `platformio-6.1.6/platformio/project/options.py` & `platformio-6.1.7/platformio/project/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     # if not all values expanded, ignore validation
     if "${" in path and "}" in path:
         return path
     if path.startswith("~"):
         path = fs.expanduser(path)
     if "$" in path:
         path = expand_dir_templates(path)
-    return fs.normalize_path(path)
+    return os.path.abspath(path)
 
 
 def get_default_core_dir():
     path = os.path.join(fs.expanduser("~"), ".platformio")
     if IS_WINDOWS:
         win_core_dir = os.path.splitdrive(path)[0] + "\\.platformio"
         if os.path.isdir(win_core_dir):
@@ -645,18 +645,18 @@
                 description="A list of check tools used for analysis",
                 type=click.Choice(["cppcheck", "clangtidy", "pvs-studio"]),
                 multiple=True,
                 default=["cppcheck"],
             ),
             ConfigEnvOption(
                 group="check",
-                name="check_patterns",
+                name="check_src_filters",
+                oldnames=["check_patterns"],
                 description=(
-                    "Configure a list of target files or directories for checking "
-                    "(Unix shell-style wildcards)"
+                    "Configure a list of target files or directories for checking"
                 ),
                 multiple=True,
             ),
             ConfigEnvOption(
                 group="check",
                 name="check_flags",
                 description="An extra flags to be passed to a check tool",
```

### Comparing `platformio-6.1.6/platformio/project/savedeps.py` & `platformio-6.1.7/platformio/project/savedeps.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/public.py` & `platformio-6.1.7/platformio/public.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/__init__.py` & `platformio-6.1.7/platformio/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/__init__.py` & `platformio-6.1.7/platformio/registry/access/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/cli.py` & `platformio-6.1.7/platformio/registry/access/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/commands/__init__.py` & `platformio-6.1.7/platformio/registry/access/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/commands/grant.py` & `platformio-6.1.7/platformio/registry/access/commands/grant.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/commands/list.py` & `platformio-6.1.7/platformio/registry/access/commands/list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/commands/private.py` & `platformio-6.1.7/platformio/registry/access/commands/private.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/access/validate.py` & `platformio-6.1.7/platformio/registry/access/validate.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/registry/client.py` & `platformio-6.1.7/platformio/registry/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,20 +138,23 @@
             "get",
             "/v3/search",
             params=params,
             x_cache_valid="1h",
             x_with_authorization=self.allowed_private_packages(),
         )
 
-    def get_package(self, type_, owner, name, version=None):
+    def get_package(self, type_, owner, name, version=None, extra_path=None):
         try:
             return self.fetch_json_data(
                 "get",
-                "/v3/packages/{owner}/{type}/{name}".format(
-                    type=type_, owner=owner.lower(), name=name.lower()
+                "/v3/packages/{owner}/{type}/{name}{extra_path}".format(
+                    type=type_,
+                    owner=owner.lower(),
+                    name=name.lower(),
+                    extra_path=extra_path or "",
                 ),
                 params=dict(version=version) if version else None,
                 x_cache_valid="1h",
                 x_with_authorization=self.allowed_private_packages(),
             )
         except HTTPClientError as exc:
             if exc.response is not None and exc.response.status_code == 404:
```

### Comparing `platformio-6.1.6/platformio/registry/mirror.py` & `platformio-6.1.7/platformio/registry/mirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from platformio import __registry_mirror_hosts__
 from platformio.cache import ContentCache
 from platformio.http import HTTPClient
 from platformio.registry.client import RegistryClient
 
 
 class RegistryFileMirrorIterator:
-
     HTTP_CLIENT_INSTANCES = {}
 
     def __init__(self, download_url):
         self.download_url = download_url
         self._url_parts = urlparse(download_url)
         self._mirror = "%s://%s" % (self._url_parts.scheme, self._url_parts.netloc)
         self._visited_mirrors = []
```

### Comparing `platformio-6.1.6/platformio/remote/__init__.py` & `platformio-6.1.7/platformio/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/ac/__init__.py` & `platformio-6.1.7/platformio/remote/ac/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/ac/base.py` & `platformio-6.1.7/platformio/remote/ac/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 # limitations under the License.
 
 from twisted.internet import defer  # pylint: disable=import-error
 from twisted.spread import pb  # pylint: disable=import-error
 
 
 class AsyncCommandBase:
-
     MAX_BUFFER_SIZE = 1024 * 1024  # 1Mb
 
     def __init__(self, options=None, on_end_callback=None):
         self.options = options or {}
         self.on_end_callback = on_end_callback
         self._buffer = b""
         self._return_code = None
```

### Comparing `platformio-6.1.6/platformio/remote/ac/process.py` & `platformio-6.1.7/platformio/remote/ac/process.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/ac/psync.py` & `platformio-6.1.7/platformio/remote/ac/psync.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/ac/serial.py` & `platformio-6.1.7/platformio/remote/ac/serial.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/cli.py` & `platformio-6.1.7/platformio/remote/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,54 +13,60 @@
 # limitations under the License.
 
 # pylint: disable=too-many-arguments, import-outside-toplevel
 # pylint: disable=inconsistent-return-statements
 
 import os
 import subprocess
+import sys
 import threading
+from site import addsitedir
 from tempfile import mkdtemp
 from time import sleep
 
 import click
 
 from platformio import fs, proc
 from platformio.device.monitor.command import (
     apply_project_monitor_options,
     device_monitor_cmd,
     get_project_options,
 )
-from platformio.package.manager.core import inject_contrib_pysite
+from platformio.package.manager.core import get_core_package_dir
 from platformio.project.exception import NotPlatformIOProjectError
 from platformio.project.options import ProjectOptions
 from platformio.run.cli import cli as cmd_run
 from platformio.test.cli import cli as test_cmd
 
 
 @click.group("remote", short_help="Remote Development")
 @click.option("-a", "--agent", multiple=True)
 @click.pass_context
 def cli(ctx, agent):
     ctx.obj = agent
-    inject_contrib_pysite()
+    # inject twisted dependencies
+    contrib_dir = get_core_package_dir("contrib-pioremote")
+    if contrib_dir not in sys.path:
+        addsitedir(contrib_dir)
+        sys.path.insert(0, contrib_dir)
 
 
 @cli.group("agent", short_help="Start a new agent or list active")
 def remote_agent():
     pass
 
 
 @remote_agent.command("start", short_help="Start agent")
 @click.option("-n", "--name")
 @click.option("-s", "--share", multiple=True, metavar="E-MAIL")
 @click.option(
     "-d",
     "--working-dir",
     envvar="PLATFORMIO_REMOTE_AGENT_DIR",
-    type=click.Path(file_okay=False, dir_okay=True, writable=True, resolve_path=True),
+    type=click.Path(file_okay=False, dir_okay=True, writable=True),
 )
 def remote_agent_start(name, share, working_dir):
     from platformio.remote.client.agent_service import RemoteAgentService
 
     RemoteAgentService(name, share, working_dir).connect()
 
 
@@ -92,17 +98,15 @@
 @click.option("-e", "--environment", multiple=True)
 @click.option("-t", "--target", multiple=True)
 @click.option("--upload-port")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=True, writable=True),
 )
 @click.option("--disable-auto-clean", is_flag=True)
 @click.option("-r", "--force-remote", is_flag=True)
 @click.option("-s", "--silent", is_flag=True)
 @click.option("-v", "--verbose", is_flag=True)
 @click.pass_obj
 @click.pass_context
@@ -114,15 +118,14 @@
     upload_port,
     project_dir,
     disable_auto_clean,
     force_remote,
     silent,
     verbose,
 ):
-
     from platformio.remote.client.run_or_test import RunOrTestClient
 
     cr = RunOrTestClient(
         "run",
         agents,
         dict(
             environment=environment,
@@ -183,17 +186,15 @@
 )
 @click.option("--upload-port")
 @click.option("--test-port")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
 )
 @click.option("-r", "--force-remote", is_flag=True)
 @click.option("--without-building", is_flag=True)
 @click.option("--without-uploading", is_flag=True)
 @click.option("--verbose", "-v", is_flag=True)
 @click.pass_obj
 @click.pass_context
@@ -207,15 +208,14 @@
     test_port,
     project_dir,
     force_remote,
     without_building,
     without_uploading,
     verbose,
 ):
-
     from platformio.remote.client.run_or_test import RunOrTestClient
 
     cr = RunOrTestClient(
         "test",
         agents,
         dict(
             environment=environment,
@@ -332,26 +332,24 @@
     is_flag=True,
     help="Diagnostics: suppress non-error messages",
 )
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(exists=True, file_okay=False, dir_okay=True, resolve_path=True),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
 @click.option(
     "-e",
     "--environment",
     help="Load configuration from `platformio.ini` and specified environment",
 )
 @click.option(
     "--sock",
-    type=click.Path(
-        exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
 )
 @click.pass_obj
 @click.pass_context
 def device_monitor(ctx, agents, **kwargs):
     from platformio.remote.client.device_monitor import DeviceMonitorClient
 
     if kwargs["sock"]:
```

### Comparing `platformio-6.1.6/platformio/remote/client/__init__.py` & `platformio-6.1.7/platformio/remote/client/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/client/agent_list.py` & `platformio-6.1.7/platformio/remote/client/agent_list.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/client/agent_service.py` & `platformio-6.1.7/platformio/remote/client/agent_service.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/client/async_base.py` & `platformio-6.1.7/platformio/remote/client/async_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     def agent_pool_ready(self):
         pass
 
     def cb_async_result(self, result):
         if self._acs_total == 0:
             self._acs_total = len(result)
-        for (success, value) in result:
+        for success, value in result:
             if not success:
                 raise pb.Error(value)
             self.acread_data(*value)
 
     def acread_data(self, agent_id, ac_id, agent_name=None):
         d = self.agentpool.callRemote("acread", agent_id, ac_id)
         d.addCallback(self.cb_acread_result, agent_id, ac_id, agent_name)
```

### Comparing `platformio-6.1.6/platformio/remote/client/base.py` & `platformio-6.1.7/platformio/remote/client/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from platformio.remote.factory.client import RemoteClientFactory
 from platformio.remote.factory.ssl import SSLContextFactory
 
 
 class RemoteClientBase(  # pylint: disable=too-many-instance-attributes
     pb.Referenceable
 ):
-
     PING_DELAY = 60
     PING_MAX_FAILURES = 3
     DEBUG = False
 
     def __init__(self):
         self.log_level = LogLevel.warn
         self.log = Logger(namespace="remote", observer=self._log_observer)
```

### Comparing `platformio-6.1.6/platformio/remote/client/device_list.py` & `platformio-6.1.7/platformio/remote/client/device_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     def agent_pool_ready(self):
         d = self.agentpool.callRemote("cmd", self.agents, "device.list")
         d.addCallback(self._cbResult)
         d.addErrback(self.cb_global_error)
 
     def _cbResult(self, result):
         data = {}
-        for (success, value) in result:
+        for success, value in result:
             if not success:
                 click.secho(value, fg="red", err=True)
                 continue
             (agent_name, devlist) = value
             data[agent_name] = devlist
 
         if self.json_output:
```

### Comparing `platformio-6.1.6/platformio/remote/client/device_monitor.py` & `platformio-6.1.7/platformio/remote/client/device_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     def send_to_server(self, data):
         self.cdm.acwrite_data(data)
 
 
 class DeviceMonitorClient(  # pylint: disable=too-many-instance-attributes
     RemoteClientBase
 ):
-
     MAX_BUFFER_SIZE = 1024 * 1024
 
     def __init__(self, agents, **kwargs):
         RemoteClientBase.__init__(self)
         self.agents = agents
         self.cmd_options = kwargs
 
@@ -92,15 +91,15 @@
         )
         d.addCallback(self._cb_device_list)
         d.addErrback(self.cb_global_error)
 
     def _cb_device_list(self, result):
         devices = []
         hwid_devindexes = []
-        for (success, value) in result:
+        for success, value in result:
             if not success:
                 click.secho(value, fg="red", err=True)
                 continue
             (agent_name, ports) = value
             for item in ports:
                 if "VID:PID" in item["hwid"]:
                     hwid_devindexes.append(len(devices))
```

### Comparing `platformio-6.1.6/platformio/remote/client/run_or_test.py` & `platformio-6.1.7/platformio/remote/client/run_or_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from platformio.compat import hashlib_encode_data
 from platformio.project.config import ProjectConfig
 from platformio.remote.client.async_base import AsyncClientBase
 from platformio.remote.projectsync import PROJECT_SYNC_STAGE, ProjectSync
 
 
 class RunOrTestClient(AsyncClientBase):
-
     MAX_ARCHIVE_SIZE = 50 * 1024 * 1024  # 50Mb
     UPLOAD_CHUNK_SIZE = 256 * 1024  # 256Kb
 
     PSYNC_SRC_EXTS = [
         "c",
         "cpp",
         "S",
@@ -143,15 +142,15 @@
         d.addErrback(self.cb_global_error)
 
         # build db index while wait for result from agent
         self.psync.rebuild_dbindex()
 
     def cb_psync_init_result(self, result):
         self._acs_total = len(result)
-        for (success, value) in result:
+        for success, value in result:
             if not success:
                 raise pb.Error(value)
             agent_id, ac_id = value
             try:
                 d = self.agentpool.callRemote(
                     "acwrite",
                     agent_id,
```

### Comparing `platformio-6.1.6/platformio/remote/client/update_core.py` & `platformio-6.1.7/platformio/remote/client/update_core.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/factory/__init__.py` & `platformio-6.1.7/platformio/remote/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/factory/client.py` & `platformio-6.1.7/platformio/remote/factory/client.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/factory/ssl.py` & `platformio-6.1.7/platformio/remote/factory/ssl.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/remote/projectsync.py` & `platformio-6.1.7/platformio/remote/projectsync.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,21 +43,21 @@
         self.items.append((path, relpath, cb_filter))
 
     def get_items(self):
         return self.items
 
     def rebuild_dbindex(self):
         self._db = {}
-        for (path, relpath, cb_filter) in self.items:
+        for path, relpath, cb_filter in self.items:
             if cb_filter and not cb_filter(path):
                 continue
             self._insert_to_db(path, relpath)
             if not isdir(path):
                 continue
-            for (root, _, files) in os.walk(path, followlinks=True):
+            for root, _, files in os.walk(path, followlinks=True):
                 for name in files:
                     self._insert_to_db(
                         join(root, name), join(relpath, root[len(path) + 1 :], name)
                     )
 
     def _insert_to_db(self, path, relpath):
         if not isfile(path):
```

### Comparing `platformio-6.1.6/platformio/run/__init__.py` & `platformio-6.1.7/platformio/run/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/run/cli.py` & `platformio-6.1.7/platformio/run/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from tabulate import tabulate
 
 from platformio import app, exception, fs, util
 from platformio.device.monitor.command import device_monitor_cmd
 from platformio.project.config import ProjectConfig
 from platformio.project.exception import ProjectError
 from platformio.project.helpers import find_project_dir_above, load_build_metadata
-from platformio.run.helpers import clean_build_dir, handle_legacy_libdeps
+from platformio.run.helpers import clean_build_dir
 from platformio.run.processor import EnvironmentProcessor
 from platformio.test.runners.base import CTX_META_TEST_IS_RUNNING
 
 # pylint: disable=too-many-arguments,too-many-locals,too-many-branches
 
 try:
     DEFAULT_JOB_NUMS = cpu_count()
@@ -43,24 +43,20 @@
 @click.option("-t", "--target", multiple=True)
 @click.option("--upload-port")
 @click.option("--monitor-port")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=True, writable=True),
 )
 @click.option(
     "-c",
     "--project-conf",
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
 )
 @click.option(
     "-j",
     "--jobs",
     type=int,
     default=DEFAULT_JOB_NUMS,
     help=(
@@ -97,41 +93,43 @@
 ):
     app.set_session_var("custom_project_conf", project_conf)
 
     # find project directory on upper level
     if os.path.isfile(project_dir):
         project_dir = find_project_dir_above(project_dir)
 
+    targets = list(target) if target else []
+    del target
+    only_monitor = targets == ["monitor"]
     is_test_running = CTX_META_TEST_IS_RUNNING in ctx.meta
+    command_failed = False
 
-    results = []
     with fs.cd(project_dir):
         config = ProjectConfig.get_instance(project_conf)
         config.validate(environment)
 
         if list_targets:
             return print_target_list(list(environment) or config.envs())
 
         # clean obsolete build dir
-        if not disable_auto_clean:
+        if not only_monitor and not disable_auto_clean:
             build_dir = config.get("platformio", "build_dir")
             try:
                 clean_build_dir(build_dir, config)
             except ProjectError as exc:
                 raise exc
             except:  # pylint: disable=bare-except
                 click.secho(
                     "Can not remove temporary directory `%s`. Please remove "
                     "it manually to avoid build issues" % build_dir,
                     fg="yellow",
                 )
 
-        handle_legacy_libdeps(project_dir, config)
-
         default_envs = config.default_envs()
+        results = []
         for env in config.envs():
             skipenv = any(
                 [
                     environment and env not in environment,
                     not environment and default_envs and env not in default_envs,
                 ]
             )
@@ -144,85 +142,92 @@
                 click.echo()
 
             results.append(
                 process_env(
                     ctx,
                     env,
                     config,
-                    environment,
-                    target,
+                    targets,
                     upload_port,
                     monitor_port,
                     jobs,
                     program_args,
                     is_test_running,
                     silent,
                     verbose,
                 )
             )
-
-    command_failed = any(r.get("succeeded") is False for r in results)
-
-    if not is_test_running and (command_failed or not silent) and len(results) > 1:
-        print_processing_summary(results, verbose)
+        command_failed = any(r.get("succeeded") is False for r in results)
+        if (
+            not is_test_running
+            and not only_monitor
+            and (command_failed or not silent)
+            and len(results) > 1
+        ):
+            print_processing_summary(results, verbose)
 
     # Reset custom project config
     app.set_session_var("custom_project_conf", None)
 
     if command_failed:
         raise exception.ReturnErrorCode(1)
+
     return True
 
 
 def process_env(
     ctx,
     name,
     config,
-    environments,
     targets,
     upload_port,
     monitor_port,
     jobs,
     program_args,
     is_test_running,
     silent,
     verbose,
 ):
     if not is_test_running and not silent:
         print_processing_header(name, config, verbose)
 
-    ep = EnvironmentProcessor(
-        ctx,
-        name,
-        config,
-        targets,
-        upload_port,
-        jobs,
-        program_args,
-        silent,
-        verbose,
-    )
-    result = {"env": name, "duration": time(), "succeeded": ep.process()}
-    result["duration"] = time() - result["duration"]
-
-    # print footer on error or when is not unit testing
-    if not is_test_running and (not silent or not result["succeeded"]):
-        print_processing_footer(result)
+    targets = targets or config.get(f"env:{name}", "targets", [])
+    only_monitor = targets == ["monitor"]
+    result = {"env": name, "duration": time(), "succeeded": True}
+
+    if not only_monitor:
+        result["succeeded"] = EnvironmentProcessor(
+            ctx,
+            name,
+            config,
+            [t for t in targets if t != "monitor"],
+            upload_port,
+            jobs,
+            program_args,
+            silent,
+            verbose,
+        ).process()
 
-    if (
-        result["succeeded"]
-        and "monitor" in ep.get_build_targets()
-        and "nobuild" not in ep.get_build_targets()
-    ):
+    if "monitor" in targets and "nobuild" not in targets:
         ctx.invoke(
             device_monitor_cmd,
             port=monitor_port,
-            environment=environments[0] if environments else None,
+            environment=name,
         )
 
+    result["duration"] = time() - result["duration"]
+
+    # print footer on error or when is not unit testing
+    if (
+        not is_test_running
+        and not only_monitor
+        and (not silent or not result["succeeded"])
+    ):
+        print_processing_footer(result)
+
     return result
 
 
 def print_processing_header(env, config, verbose=False):
     env_dump = []
     for k, v in config.items(env=env):
         if verbose or k in ("platform", "framework", "board"):
```

### Comparing `platformio-6.1.6/platformio/run/processor.py` & `platformio-6.1.7/platformio/run/processor.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from platformio.package.commands.install import install_project_env_dependencies
 from platformio.platform.factory import PlatformFactory
 from platformio.project.exception import UndefinedEnvPlatformError
+from platformio.run.helpers import KNOWN_ALLCLEAN_TARGETS
 from platformio.test.runners.base import CTX_META_TEST_RUNNING_NAME
 
 # pylint: disable=too-many-instance-attributes
 
 
 class EnvironmentProcessor:
     def __init__(  # pylint: disable=too-many-arguments
@@ -32,15 +33,15 @@
         program_args,
         silent,
         verbose,
     ):
         self.cmd_ctx = cmd_ctx
         self.name = name
         self.config = config
-        self.targets = [str(t) for t in targets]
+        self.targets = targets
         self.upload_port = upload_port
         self.jobs = jobs
         self.program_args = program_args
         self.silent = silent
         self.verbose = verbose
         self.options = config.items(env=name, as_dict=True)
 
@@ -57,38 +58,34 @@
             ]
 
         if self.upload_port:
             # override upload port with a custom from CLI
             variables["upload_port"] = self.upload_port
         return variables
 
-    def get_build_targets(self):
-        return (
-            self.targets
-            if self.targets
-            else self.config.get("env:" + self.name, "targets", [])
-        )
-
     def process(self):
         if "platform" not in self.options:
             raise UndefinedEnvPlatformError(self.name)
 
         build_vars = self.get_build_variables()
-        build_targets = list(self.get_build_targets())
-
-        # skip monitor target, we call it above
-        if "monitor" in build_targets:
-            build_targets.remove("monitor")
-
-        if not set(["clean", "cleanall"]) & set(build_targets):
-            install_project_env_dependencies(
-                self.name,
-                {
-                    "project_targets": build_targets,
-                    "piotest_running_name": build_vars.get("piotest_running_name"),
-                },
-            )
+        is_clean = set(KNOWN_ALLCLEAN_TARGETS) & set(self.targets)
+        build_targets = [t for t in self.targets if t not in KNOWN_ALLCLEAN_TARGETS]
 
+        # pre-clean
+        if is_clean:
+            result = PlatformFactory.new(
+                self.options["platform"], autoinstall=True
+            ).run(build_vars, self.targets, self.silent, self.verbose, self.jobs)
+            if not build_targets:
+                return result["returncode"] == 0
+
+        install_project_env_dependencies(
+            self.name,
+            {
+                "project_targets": self.targets,
+                "piotest_running_name": build_vars.get("piotest_running_name"),
+            },
+        )
         result = PlatformFactory.new(self.options["platform"], autoinstall=True).run(
             build_vars, build_targets, self.silent, self.verbose, self.jobs
         )
         return result["returncode"] == 0
```

### Comparing `platformio-6.1.6/platformio/system/__init__.py` & `platformio-6.1.7/platformio/system/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/system/cli.py` & `platformio-6.1.7/platformio/system/cli.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/system/commands/__init__.py` & `platformio-6.1.7/platformio/system/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/system/commands/completion.py` & `platformio-6.1.7/platformio/system/commands/completion.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 @system_completion_cmd.command(
     "install", short_help="Install shell completion files/code"
 )
 @click.argument("shell", type=click.Choice([t.value for t in ShellType]))
 @click.option(
     "--path",
-    type=click.Path(file_okay=True, dir_okay=False, readable=True, resolve_path=True),
+    type=click.Path(file_okay=True, dir_okay=False, readable=True),
     help="Custom installation path of the code to be evaluated by the shell. "
     "The standard installation path is used by default.",
 )
 def system_completion_install(shell, path):
     shell = ShellType(shell)
     path = path or get_completion_install_path(shell)
     install_completion_code(shell, path)
@@ -50,15 +50,15 @@
 
 @system_completion_cmd.command(
     "uninstall", short_help="Uninstall shell completion files/code"
 )
 @click.argument("shell", type=click.Choice([t.value for t in ShellType]))
 @click.option(
     "--path",
-    type=click.Path(file_okay=True, dir_okay=False, readable=True, resolve_path=True),
+    type=click.Path(file_okay=True, dir_okay=False, readable=True),
     help="Custom installation path of the code to be evaluated by the shell. "
     "The standard installation path is used by default.",
 )
 def system_completion_uninstall(shell, path):
     shell = ShellType(shell)
     path = path or get_completion_install_path(shell)
     uninstall_completion_code(shell, path)
```

### Comparing `platformio-6.1.6/platformio/system/commands/info.py` & `platformio-6.1.7/platformio/system/commands/info.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/system/commands/prune.py` & `platformio-6.1.7/platformio/system/commands/prune.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/system/completion.py` & `platformio-6.1.7/platformio/system/completion.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/system/prune.py` & `platformio-6.1.7/platformio/system/prune.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/telemetry.py` & `platformio-6.1.7/platformio/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,14 @@
             del self._params[name]
 
     def send(self, hittype):
         raise NotImplementedError()
 
 
 class MeasurementProtocol(TelemetryBase):
-
     TID = "UA-1768265-9"
     PARAMS_MAP = {
         "screen_name": "cd",
         "event_category": "ec",
         "event_action": "ea",
         "event_label": "el",
         "event_value": "ev",
@@ -102,26 +101,14 @@
                 return
             if any(("@" in arg, "/" in arg, "\\" in arg)):
                 arg = "***"
             args.append(arg.lower())
         self["cd3"] = " ".join(args)
 
     def _prefill_custom_data(self):
-        def _filter_args(items):
-            result = []
-            stop = False
-            for item in items:
-                item = str(item).lower()
-                result.append(item)
-                if stop:
-                    break
-                if item == "account":
-                    stop = True
-            return result
-
         caller_id = str(app.get_session_var("caller_id"))
         self["cd1"] = util.get_systype()
         self["cd4"] = 1 if (not is_ci() and (caller_id or not is_container())) else 0
         if caller_id:
             self["cd5"] = caller_id.lower()
 
     def _prefill_screen_name(self):
@@ -197,15 +184,14 @@
         if "qt" in self._params and isinstance(self["qt"], float):
             self["qt"] = int((time() - self["qt"]) * 1000)
         MPDataPusher().push(self._params)
 
 
 @util.singleton
 class MPDataPusher:
-
     MAX_WORKERS = 5
 
     def __init__(self):
         self._queue = queue.LifoQueue()
         self._failedque = deque()
         self._http_session = HTTPSession()
         self._http_offline = False
```

### Comparing `platformio-6.1.6/platformio/test/__init__.py` & `platformio-6.1.7/platformio/test/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/cli.py` & `platformio-6.1.7/platformio/test/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,24 +44,20 @@
 )
 @click.option("--upload-port")
 @click.option("--test-port")
 @click.option(
     "-d",
     "--project-dir",
     default=os.getcwd,
-    type=click.Path(
-        exists=True, file_okay=False, dir_okay=True, writable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True),
 )
 @click.option(
     "-c",
     "--project-conf",
-    type=click.Path(
-        exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True
-    ),
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
 )
 @click.option("--without-building", is_flag=True)
 @click.option("--without-uploading", is_flag=True)
 @click.option("--without-testing", is_flag=True)
 @click.option("--no-reset", is_flag=True)
 @click.option(
     "--monitor-rts",
@@ -79,16 +75,16 @@
     "-a",
     "--program-arg",
     "program_args",
     multiple=True,
     help="A program argument (multiple are allowed)",
 )
 @click.option("--list-tests", is_flag=True)
-@click.option("--json-output-path", type=click.Path(resolve_path=True))
-@click.option("--junit-output-path", type=click.Path(resolve_path=True))
+@click.option("--json-output-path", type=click.Path())
+@click.option("--junit-output-path", type=click.Path())
 @click.option(
     "--verbose",
     "-v",
     count=True,
     help="Increase verbosity level, maximum is 3 levels (-vvv), see docs for details",
 )
 @click.pass_context
```

### Comparing `platformio-6.1.6/platformio/test/exception.py` & `platformio-6.1.7/platformio/test/exception.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 
 class UnitTestError(PlatformioException):
     pass
 
 
 class TestDirNotExistsError(UnitTestError, UserSideException):
-
     MESSAGE = (
         "A test folder '{0}' does not exist.\nPlease create 'test' "
         "directory in the project root and put a test suite.\n"
         "More details about Unit "
         "Testing: https://docs.platformio.org/en/latest/advanced/"
         "unit-testing/index.html"
     )
```

### Comparing `platformio-6.1.6/platformio/test/helpers.py` & `platformio-6.1.7/platformio/test/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 def list_test_suites(project_config, environments, filters, ignores):
     result = []
     test_dir = project_config.get("platformio", "test_dir")
     default_envs = project_config.default_envs()
     test_names = list_test_names(project_config)
     for env_name in project_config.envs():
         for test_name in test_names:
-
             # filter and ignore patterns
             patterns = dict(filter=list(filters), ignore=list(ignores))
             for key, value in patterns.items():
                 if value:  # overridden from CLI
                     continue
                 patterns[key].extend(  # pylint: disable=unnecessary-dict-index-lookup
                     project_config.get(f"env:{env_name}", f"test_{key}", [])
```

### Comparing `platformio-6.1.6/platformio/test/reports/__init__.py` & `platformio-6.1.7/platformio/test/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/reports/base.py` & `platformio-6.1.7/platformio/test/reports/base.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/reports/json.py` & `platformio-6.1.7/platformio/test/reports/json.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/reports/junit.py` & `platformio-6.1.7/platformio/test/reports/junit.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/reports/stdout.py` & `platformio-6.1.7/platformio/test/reports/stdout.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/result.py` & `platformio-6.1.7/platformio/test/result.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/runners/__init__.py` & `platformio-6.1.7/platformio/test/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/runners/base.py` & `platformio-6.1.7/platformio/test/runners/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import click
 
 from platformio.exception import ReturnErrorCode
 from platformio.platform.factory import PlatformFactory
 from platformio.test.exception import UnitTestSuiteError
 from platformio.test.result import TestCase, TestStatus
-from platformio.test.runners.readers.program import ProgramTestOutputReader
+from platformio.test.runners.readers.native import NativeTestOutputReader
 from platformio.test.runners.readers.serial import SerialTestOutputReader
 
 CTX_META_TEST_IS_RUNNING = __name__ + ".test_running"
 CTX_META_TEST_RUNNING_NAME = __name__ + ".test_running_name"
 
 
 class TestRunnerOptions:  # pylint: disable=too-many-instance-attributes
@@ -50,15 +50,14 @@
         self.no_reset = no_reset
         self.monitor_rts = monitor_rts
         self.monitor_dtr = monitor_dtr
         self.program_args = program_args
 
 
 class TestRunnerBase:
-
     NAME = None
     EXTRA_LIB_DEPS = None
     TESTCASE_PARSE_RE = None
 
     def __init__(self, test_suite, project_config, options=None):
         self.test_suite = test_suite
         self.options = options
@@ -157,24 +156,24 @@
             ) from exc
 
     def stage_testing(self):
         if self.options.without_testing:
             return None
         click.secho("Testing...", bold=True)
         test_port = self.get_test_port()
-        program_conds = [
+        native_conds = [
             not self.platform.is_embedded()
             and (not test_port or "://" not in test_port),
             self.project_config.get(
                 f"env:{self.test_suite.env_name}", "test_testing_command"
             ),
         ]
         reader = (
-            ProgramTestOutputReader(self)
-            if any(program_conds)
+            NativeTestOutputReader(self)
+            if any(native_conds)
             else SerialTestOutputReader(self)
         )
         return reader.begin()
 
     def teardown(self):
         pass
```

### Comparing `platformio-6.1.6/platformio/test/runners/doctest.py` & `platformio-6.1.7/platformio/test/runners/doctest.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,14 @@
             if index == -1:
                 continue
             self._tmp_tc.status = status
             self._tmp_tc.message = line[index + len(token) + 3 :].strip() or None
 
 
 class DoctestTestRunner(TestRunnerBase):
-
     EXTRA_LIB_DEPS = ["doctest/doctest@^2.4.9"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._tc_parser = DoctestTestCaseParser()
 
     def on_testing_line_output(self, line):
```

### Comparing `platformio-6.1.6/platformio/test/runners/factory.py` & `platformio-6.1.7/platformio/test/runners/factory.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/runners/googletest.py` & `platformio-6.1.7/platformio/test/runners/googletest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import click
 
 from platformio.test.result import TestCase, TestCaseSource, TestStatus
 from platformio.test.runners.base import TestRunnerBase
 
 
 class GoogletestTestCaseParser:
-
     # Examples:
     # [ RUN      ] FooTest.Bar
     # ...
     # [  FAILED  ] FooTest.Bar (0 ms)
     STATUS__NAME_RE = r"^\[\s+(?P<status>[A-Z]+)\s+\]\s+(?P<name>[^\(\s]+)"
 
     # Examples:
@@ -85,15 +84,14 @@
                 ),
                 (match.group("message") or "").strip() or None,
             )
         return (None, None)
 
 
 class GoogletestTestRunner(TestRunnerBase):
-
     EXTRA_LIB_DEPS = ["google/googletest@^1.12.1"]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._tc_parser = GoogletestTestCaseParser()
         os.environ["GTEST_COLOR"] = "no"  # disable ANSI symbols
```

### Comparing `platformio-6.1.6/platformio/test/runners/readers/__init__.py` & `platformio-6.1.7/platformio/test/runners/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `platformio-6.1.6/platformio/test/runners/readers/program.py` & `platformio-6.1.7/platformio/test/runners/readers/native.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 from platformio.compat import (
     IS_WINDOWS,
     aio_get_running_loop,
     get_filesystem_encoding,
     get_locale_encoding,
 )
+from platformio.project.helpers import load_build_metadata
 from platformio.test.exception import UnitTestError
 
 EXITING_TIMEOUT = 5  # seconds
 
 
 class ProgramProcessProtocol(asyncio.SubprocessProtocol):
     def __init__(self, test_runner, exit_future):
@@ -52,15 +53,15 @@
     def _stop_testing(self):
         if not self.exit_future.done():
             self.exit_future.set_result(True)
         if self._exit_timer:
             self._exit_timer.cancel()
 
 
-class ProgramTestOutputReader:
+class NativeTestOutputReader:
     def __init__(self, test_runner):
         self.test_runner = test_runner
         self.aio_loop = (
             asyncio.ProactorEventLoop() if IS_WINDOWS else asyncio.new_event_loop()
         )
         asyncio.set_event_loop(self.aio_loop)
 
@@ -74,14 +75,21 @@
         cmd = [
             os.path.join(
                 build_dir,
                 self.test_runner.test_suite.env_name,
                 "program.exe" if IS_WINDOWS else "program",
             )
         ]
+        # if user changed PROGNAME
+        if not os.path.exists(cmd[0]):
+            build_data = load_build_metadata(
+                os.getcwd(), self.test_runner.test_suite.env_name, cache=True
+            )
+            if build_data:
+                cmd[0] = build_data["prog_path"]
         if self.test_runner.options.program_args:
             cmd.extend(self.test_runner.options.program_args)
         return cmd
 
     async def gather_results(self):
         exit_future = asyncio.Future(loop=self.aio_loop)
         transport, _ = await self.aio_loop.subprocess_exec(
```

### Comparing `platformio-6.1.6/platformio/test/runners/readers/serial.py` & `platformio-6.1.7/platformio/test/runners/readers/serial.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import serial
 
 from platformio.device.finder import SerialPortFinder
 from platformio.exception import UserSideException
 
 
 class SerialTestOutputReader:
-
     SERIAL_TIMEOUT = 600
 
     def __init__(self, test_runner):
         self.test_runner = test_runner
 
     def begin(self):
         click.echo(
@@ -43,15 +42,15 @@
                 timeout=self.SERIAL_TIMEOUT,
             )
             ser.rts = self.test_runner.options.monitor_rts
             ser.dtr = self.test_runner.options.monitor_dtr
             ser.open()
         except serial.SerialException as exc:
             click.secho(str(exc), fg="red", err=True)
-            return None
+            return
 
         if not self.test_runner.options.no_reset:
             ser.flushInput()
             ser.setDTR(False)
             ser.setRTS(False)
             sleep(0.1)
             ser.setDTR(True)
```

### Comparing `platformio-6.1.6/platformio/test/runners/unity.py` & `platformio-6.1.7/platformio/test/runners/unity.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 from platformio.test.exception import UnitTestSuiteError
 from platformio.test.result import TestCase, TestCaseSource, TestStatus
 from platformio.test.runners.base import TestRunnerBase
 from platformio.util import strip_ansi_codes
 
 
 class UnityTestRunner(TestRunnerBase):
-
     EXTRA_LIB_DEPS = ["throwtheswitch/Unity@^2.5.2"]
 
     # Examples:
     # test/test_foo.cpp:44:test_function_foo:FAIL: Expected 32 Was 33
     # test/group/test_foo/test_main.cpp:5:test::dummy:FAIL: Expression Evaluated To FALSE
     TESTCASE_PARSE_RE = re.compile(
         r"(?P<source_file>[^:]+):(?P<source_line>\d+):(?P<name>[^\s]+):"
@@ -111,15 +110,15 @@
 $framework_config_code
     """
 
     UNITY_FRAMEWORK_CONFIG = dict(
         native=dict(
             code="""
 #include <stdio.h>
-void unityOutputStart(unsigned long baudrate) { }
+void unityOutputStart(unsigned long baudrate) { (void) baudrate; }
 void unityOutputChar(unsigned int c) { putchar(c); }
 void unityOutputFlush(void) { fflush(stdout); }
 void unityOutputComplete(void) { }
         """,
             language="c",
         ),
         arduino=dict(
@@ -152,25 +151,25 @@
 void unityOutputComplete(void) { }
         """,
             language="cpp",
         ),
         espidf=dict(
             code="""
 #include <stdio.h>
-void unityOutputStart(unsigned long baudrate) { }
+void unityOutputStart(unsigned long baudrate) { (void) baudrate; }
 void unityOutputChar(unsigned int c) { putchar(c); }
 void unityOutputFlush(void) { fflush(stdout); }
 void unityOutputComplete(void) { }
         """,
             language="c",
         ),
         zephyr=dict(
             code="""
 #include <sys/printk.h>
-void unityOutputStart(unsigned long baudrate) { }
+void unityOutputStart(unsigned long baudrate) { (void) baudrate; }
 void unityOutputChar(unsigned int c) { printk("%c", c); }
 void unityOutputFlush(void) { }
 void unityOutputComplete(void) { }
         """,
             language="c",
         ),
         legacy_custom_transport=dict(
```

### Comparing `platformio-6.1.6/platformio/util.py` & `platformio-6.1.7/platformio/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
 
 
 class RetryStopException(RetryException):
     pass
 
 
 class retry:
-
     RetryNextException = RetryNextException
     RetryStopException = RetryStopException
 
     def __init__(self, timeout=0, step=0.25):
         self.timeout = timeout
         self.step = step
```

### Comparing `platformio-6.1.6/platformio.egg-info/PKG-INFO` & `platformio-6.1.7/platformio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: platformio
-Version: 6.1.6
+Version: 6.1.7
 Summary: A professional collaborative platform for embedded development. Cross-platform IDE and Unified Debugger. Static Code Analyzer and Remote Unit Testing. Multi-platform and Multi-architecture Build System. Firmware File Explorer and Memory Inspection. IoT, Arduino, CMSIS, ESP-IDF, FreeRTOS, libOpenCM3, mbedOS, Pulp OS, SPL, STM32Cube, Zephyr RTOS, ARM, AVR, Espressif (ESP8266/ESP32), FPGA, MCS-51 (8051), MSP430, Nordic (nRF51/nRF52), NXP i.MX RT, PIC32, RISC-V, STMicroelectronics (STM8/STM32), Teensy
 Home-page: https://platformio.org
 Author: PlatformIO Labs
 Author-email: contact@piolabs.com
 License: Apache Software License
 Keywords: iot,embedded,arduino,mbed,esp8266,esp32,fpga,firmware,continuous-integration,cloud-ide,avr,arm,ide,unit-testing,hardware,verilog,microcontroller,debug
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
@@ -119,8 +118,7 @@
 
 The PlatformIO is licensed under the permissive Apache 2.0 license,
 so you can use it in both commercial and personal projects with confidence.
 
 .. image:: https://raw.githubusercontent.com/vshymanskyy/StandWithUkraine/main/banner-direct.svg
     :target: https://github.com/vshymanskyy/StandWithUkraine/blob/main/docs/README.md
     :alt:  SWUbanner
-
```

### Comparing `platformio-6.1.6/platformio.egg-info/SOURCES.txt` & `platformio-6.1.7/platformio.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -64,14 +64,19 @@
 platformio/assets/templates/ide-projects/eclipse/.cproject.tpl
 platformio/assets/templates/ide-projects/eclipse/.project.tpl
 platformio/assets/templates/ide-projects/eclipse/.settings/PlatformIO Debugger.launch.tpl
 platformio/assets/templates/ide-projects/eclipse/.settings/language.settings.xml.tpl
 platformio/assets/templates/ide-projects/eclipse/.settings/org.eclipse.cdt.core.prefs.tpl
 platformio/assets/templates/ide-projects/emacs/.ccls.tpl
 platformio/assets/templates/ide-projects/emacs/.gitignore.tpl
+platformio/assets/templates/ide-projects/netbeans/nbproject/configurations.xml.tpl
+platformio/assets/templates/ide-projects/netbeans/nbproject/project.xml.tpl
+platformio/assets/templates/ide-projects/netbeans/nbproject/private/configurations.xml.tpl
+platformio/assets/templates/ide-projects/netbeans/nbproject/private/launcher.properties.tpl
+platformio/assets/templates/ide-projects/netbeans/nbproject/private/private.xml.tpl
 platformio/assets/templates/ide-projects/qtcreator/.gitignore.tpl
 platformio/assets/templates/ide-projects/qtcreator/Makefile.tpl
 platformio/assets/templates/ide-projects/qtcreator/platformio.cflags.tpl
 platformio/assets/templates/ide-projects/qtcreator/platformio.config.tpl
 platformio/assets/templates/ide-projects/qtcreator/platformio.creator.tpl
 platformio/assets/templates/ide-projects/qtcreator/platformio.cxxflags.tpl
 platformio/assets/templates/ide-projects/qtcreator/platformio.files.tpl
@@ -85,15 +90,14 @@
 platformio/assets/templates/ide-projects/vscode/.gitignore.tpl
 platformio/assets/templates/ide-projects/vscode/.vscode/c_cpp_properties.json.tpl
 platformio/assets/templates/ide-projects/vscode/.vscode/extensions.json.tpl
 platformio/assets/templates/ide-projects/vscode/.vscode/launch.json.tpl
 platformio/builder/__init__.py
 platformio/builder/main.py
 platformio/builder/tools/__init__.py
-platformio/builder/tools/compilation_db.py
 platformio/builder/tools/pioasm.py
 platformio/builder/tools/piobuild.py
 platformio/builder/tools/piohooks.py
 platformio/builder/tools/pioino.py
 platformio/builder/tools/piointegration.py
 platformio/builder/tools/piolib.py
 platformio/builder/tools/piomaxlen.py
@@ -153,25 +157,26 @@
 platformio/device/monitor/filters/base.py
 platformio/device/monitor/filters/hexlify.py
 platformio/device/monitor/filters/log2file.py
 platformio/device/monitor/filters/send_on_enter.py
 platformio/device/monitor/filters/time.py
 platformio/home/__init__.py
 platformio/home/cli.py
-platformio/home/helpers.py
 platformio/home/run.py
 platformio/home/rpc/__init__.py
 platformio/home/rpc/server.py
 platformio/home/rpc/handlers/__init__.py
 platformio/home/rpc/handlers/account.py
 platformio/home/rpc/handlers/app.py
+platformio/home/rpc/handlers/base.py
 platformio/home/rpc/handlers/ide.py
 platformio/home/rpc/handlers/misc.py
 platformio/home/rpc/handlers/os.py
 platformio/home/rpc/handlers/piocore.py
+platformio/home/rpc/handlers/platform.py
 platformio/home/rpc/handlers/project.py
 platformio/home/rpc/handlers/registry.py
 platformio/package/__init__.py
 platformio/package/cli.py
 platformio/package/download.py
 platformio/package/exception.py
 platformio/package/lockfile.py
@@ -285,9 +290,10 @@
 platformio/test/runners/__init__.py
 platformio/test/runners/base.py
 platformio/test/runners/doctest.py
 platformio/test/runners/factory.py
 platformio/test/runners/googletest.py
 platformio/test/runners/unity.py
 platformio/test/runners/readers/__init__.py
-platformio/test/runners/readers/program.py
-platformio/test/runners/readers/serial.py
+platformio/test/runners/readers/native.py
+platformio/test/runners/readers/serial.py
+tests/test_examples.py
```

### Comparing `platformio-6.1.6/setup.py` & `platformio-6.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,24 +32,25 @@
     "bottle==0.12.*",
     "click%s" % ("==8.0.4" if PY36 else ">=8.0.4,<9"),
     "colorama",
     "marshmallow==%s" % ("3.14.1" if PY36 else "3.*"),
     "pyelftools>=0.27,<1",
     "pyserial==3.5.*",  # keep in sync "device/monitor/terminal.py"
     "requests==2.*",
+    "urllib3<2", # issue 4614: urllib3 v2.0 only supports OpenSSL 1.1.1+
     "requests==%s" % ("2.27.1" if PY36 else "2.*"),
     "semantic_version==2.10.*",
     "tabulate==%s" % ("0.8.10" if PY36 else "0.9.*"),
 ]
 
 home_requirements = [
-    "aiofiles==%s" % ("0.8.0" if PY36 else "22.1.*"),
+    "aiofiles==%s" % ("0.8.0" if PY36 else "23.1.*"),
     "ajsonrpc==1.*",
-    "starlette==%s" % ("0.19.1" if PY36 else "0.23.*"),
-    "uvicorn==%s" % ("0.16.0" if PY36 else "0.20.*"),
+    "starlette==%s" % ("0.19.1" if PY36 else "0.26.*"),
+    "uvicorn==%s" % ("0.16.0" if PY36 else "0.22.*"),
     "wsproto==%s" % ("1.0.0" if PY36 else "1.2.*"),
 ]
 
 setup(
     name=__title__,
     version=__version__,
     description=__description__,
@@ -63,14 +64,16 @@
     packages=find_packages(include=["platformio", "platformio.*"]),
     package_data={
         "platformio": [
             "assets/system/99-platformio-udev.rules",
             "assets/templates/ide-projects/*/*.tpl",
             "assets/templates/ide-projects/*/.*.tpl",  # include hidden files
             "assets/templates/ide-projects/*/.*/*.tpl",  # include hidden folders
+            "assets/templates/ide-projects/*/*/*.tpl",  # NetBeans
+            "assets/templates/ide-projects/*/*/*/*.tpl", # NetBeans
         ]
     },
     entry_points={
         "console_scripts": [
             "platformio = platformio.__main__:main",
             "pio = platformio.__main__:main",
             "piodebuggdb = platformio.__main__:debug_gdb_main",
```

