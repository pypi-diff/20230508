# Comparing `tmp/pnu_libpnu-1.1.2.tar.gz` & `tmp/pnu-libpnu-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnu_libpnu-1.1.2.tar", last modified: Sat Dec 17 15:21:09 2022, max compression
+gzip compressed data, was "pnu-libpnu-1.2.0.tar", last modified: Mon May  8 11:44:24 2023, max compression
```

## Comparing `pnu_libpnu-1.1.2.tar` & `pnu-libpnu-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2022-12-17 15:21:09.707317 pnu_libpnu-1.1.2/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2022-02-27 16:34:31.000000 pnu_libpnu-1.1.2/License
--rw-r--r--   0 hubert    (1001) hubert    (1001)     4077 2022-12-17 15:21:09.707415 pnu_libpnu-1.1.2/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)     2752 2022-03-27 08:41:00.000000 pnu_libpnu-1.1.2/README.md
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2022-12-17 15:21:09.706039 pnu_libpnu-1.1.2/man/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1259 2022-12-17 15:21:01.000000 pnu_libpnu-1.1.2/man/libpnu.3.gz
--rw-r--r--   0 hubert    (1001) hubert    (1001)      104 2022-02-27 16:34:15.000000 pnu_libpnu-1.1.2/pyproject.toml
--rw-r--r--   0 hubert    (1001) hubert    (1001)     1362 2022-12-17 15:21:09.708076 pnu_libpnu-1.1.2/setup.cfg
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2022-12-17 15:21:09.705045 pnu_libpnu-1.1.2/src/
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2022-12-17 15:21:09.706421 pnu_libpnu-1.1.2/src/libpnu/
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2022-02-27 16:34:15.000000 pnu_libpnu-1.1.2/src/libpnu/__init__.py
--rwxr-xr-x   0 hubert    (1001) hubert    (1001)     4566 2022-12-17 15:19:49.000000 pnu_libpnu-1.1.2/src/libpnu/main.py
-drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2022-12-17 15:21:09.707183 pnu_libpnu-1.1.2/src/pnu_libpnu.egg-info/
--rw-r--r--   0 hubert    (1001) hubert    (1001)     4077 2022-12-17 15:21:09.000000 pnu_libpnu-1.1.2/src/pnu_libpnu.egg-info/PKG-INFO
--rw-r--r--   0 hubert    (1001) hubert    (1001)      252 2022-12-17 15:21:09.000000 pnu_libpnu-1.1.2/src/pnu_libpnu.egg-info/SOURCES.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2022-12-17 15:21:09.000000 pnu_libpnu-1.1.2/src/pnu_libpnu.egg-info/dependency_links.txt
--rw-r--r--   0 hubert    (1001) hubert    (1001)        7 2022-12-17 15:21:09.000000 pnu_libpnu-1.1.2/src/pnu_libpnu.egg-info/top_level.txt
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-08 11:44:24.617252 pnu-libpnu-1.2.0/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1461 2022-02-27 16:34:31.000000 pnu-libpnu-1.2.0/License
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     4777 2023-05-08 11:44:24.617357 pnu-libpnu-1.2.0/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     3401 2023-05-08 11:39:12.000000 pnu-libpnu-1.2.0/README.md
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-08 11:44:24.616088 pnu-libpnu-1.2.0/man/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1459 2023-05-08 11:44:16.000000 pnu-libpnu-1.2.0/man/libpnu.3.gz
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      104 2022-02-27 16:34:15.000000 pnu-libpnu-1.2.0/pyproject.toml
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     1402 2023-05-08 11:44:24.618016 pnu-libpnu-1.2.0/setup.cfg
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-08 11:44:24.615184 pnu-libpnu-1.2.0/src/
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-08 11:44:24.616439 pnu-libpnu-1.2.0/src/libpnu/
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)       60 2022-02-27 16:34:15.000000 pnu-libpnu-1.2.0/src/libpnu/__init__.py
+-rwxr-xr-x   0 hubert    (1001) hubert    (1001)     6183 2023-05-08 11:32:08.000000 pnu-libpnu-1.2.0/src/libpnu/main.py
+drwxr-xr-x   0 hubert    (1001) hubert    (1001)        0 2023-05-08 11:44:24.617136 pnu-libpnu-1.2.0/src/pnu_libpnu.egg-info/
+-rw-r--r--   0 hubert    (1001) hubert    (1001)     4777 2023-05-08 11:44:24.000000 pnu-libpnu-1.2.0/src/pnu_libpnu.egg-info/PKG-INFO
+-rw-r--r--   0 hubert    (1001) hubert    (1001)      252 2023-05-08 11:44:24.000000 pnu-libpnu-1.2.0/src/pnu_libpnu.egg-info/SOURCES.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        1 2023-05-08 11:44:24.000000 pnu-libpnu-1.2.0/src/pnu_libpnu.egg-info/dependency_links.txt
+-rw-r--r--   0 hubert    (1001) hubert    (1001)        7 2023-05-08 11:44:24.000000 pnu-libpnu-1.2.0/src/pnu_libpnu.egg-info/top_level.txt
```

### Comparing `pnu_libpnu-1.1.2/License` & `pnu-libpnu-1.2.0/License`

 * *Files identical despite different names*

### Comparing `pnu_libpnu-1.1.2/PKG-INFO` & `pnu-libpnu-1.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pnu_libpnu
-Version: 1.1.2
+Name: pnu-libpnu
+Version: 1.2.0
 Summary: Common utility functions for the PNU project
 Home-page: https://github.com/HubTou/libpnu/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/libpnu/issues
 Keywords: pnu-project
@@ -21,21 +21,22 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: License
 
 # Installation
-pip install [pnu-libpnu](https://pypi.org/project/pnu-libpnu/)
+This library will be installed as a dependency by other PNU utilities.
 
 # LIBPNU(3)
 
 ## NAME
 libpnu — Common utility functions for the PNU project
 
 ## SYNOPSIS
@@ -43,50 +44,62 @@
 
 *libpnu*.**initialize_debugging**(String *program_name*)
 
 *libpnu*.**handle_interrupt_signals**(Function *handler_function*)
 
 String *libpnu*.**get_home_directory**()
 
+String *libpnu*.**get_caching_directory**(String *name*)
+
 List *libpnu*.**locate_directory**(String *directory*)
 
+List *libpnu*.**load_strings_from_file**(String *filename*)
+
 ## DESCRIPTION
 The **initialize_debugging()** function sets up the Python logging module with a syslog style kind of console log using *program_name* as the program name.
 By default, the logging level is set at WARNING or more, but can be lowered by calling **logging.disable()**,
 for example with the *logging.NOTSET* parameter to get DEBUG or more logging level.
 
 The **handle_interrupt_signals()** function calls the specified *handler_function* to process the SIGINT and SIGPIPE signals,
 usually to avoid an ugly trace dump to the console in case of interrupt (Control-C pressed or broken pipe).
 
 The **get_home_directory()** function returns the location of the user's home directory in a string
 depending on the operating system used (Unix, Windows).
 
+The **get_caching_directory()** function returns the location of a user writable directory for caching files in a string
+depending on the operating system used (Unix, Windows).
+The provided *name* will be the last directory part of this location.
+
 The **locate_directory()** function searches the specified *directory* in a variety of possible other directories,
 depending on the operating system used (Unix, Windows) and the fact that a package can be user or system installed.
 It is intended to be used when the directory can't be directly found, and returns a list of paths where the directory searched has been found.
 
 For example, if the argument is "/usr/local/etc/man.d", we'll search for "usr/local/etc/man.d", "local/etc/man.d", "etc/man.d" (more likely) and "man.d"
 in a list of user's local Python package directories
 ("$HOME/.local" on Unix, "$APPDATA/python", "$HOMEPATH/appdata/roaming/python", "$USERPROFILE/appdata/roaming/python" on Windows)
 and system wide Python package base directories (given by *sys.base_prefix*: "/usr/local" on Unix, "C:/Program Files/Python3x" on Windows).
 
+The **load_strings_from_file()** function returns a list of strings from the given *filename*,
+filtering out blank or commented lines, as well as end-of-line comments (with '#' being the comment character).
+
 ## ENVIRONMENT
-The following environment variables can be used to identify the user identity and home directory.
+The following environment variables can be used to identify the user identity and home directory,
+or find a caching directory.
 
-On Unix: *HOME*, *LOGNAME*, *USER*, *LNAME* and *USERNAME*.
+On Unix: *HOME*, *LNAME*, *LOGNAME*, *TMP*, *TMPDIR*, *USER* and *USERNAME*.
 
-On Windows: *APPDATA*, *HOME*, *HOMEPATH* and *USERPROFILE*.
+On Windows: *APPDATA*, *HOME*, *HOMEPATH*, *LOCALAPPDATA*, *TMP* and *USERPROFILE*.
 
 ## STANDARDS
 The **libpnu** library is not a standard UNIX one.
 
 It tries to follow the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide for [Python](https://www.python.org/) code.
 
 ## PORTABILITY
-To be tested under Windows.
+Tested OK under Windows.
 
 ## HISTORY
 This library was made for the [PNU project](https://github.com/HubTou/PNU).
 
 ## LICENSE
 It is available under the [3-clause BSD license](https://opensource.org/licenses/BSD-3-Clause).
```

### Comparing `pnu_libpnu-1.1.2/README.md` & `pnu-libpnu-1.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Installation
-pip install [pnu-libpnu](https://pypi.org/project/pnu-libpnu/)
+This library will be installed as a dependency by other PNU utilities.
 
 # LIBPNU(3)
 
 ## NAME
 libpnu — Common utility functions for the PNU project
 
 ## SYNOPSIS
@@ -11,50 +11,62 @@
 
 *libpnu*.**initialize_debugging**(String *program_name*)
 
 *libpnu*.**handle_interrupt_signals**(Function *handler_function*)
 
 String *libpnu*.**get_home_directory**()
 
+String *libpnu*.**get_caching_directory**(String *name*)
+
 List *libpnu*.**locate_directory**(String *directory*)
 
+List *libpnu*.**load_strings_from_file**(String *filename*)
+
 ## DESCRIPTION
 The **initialize_debugging()** function sets up the Python logging module with a syslog style kind of console log using *program_name* as the program name.
 By default, the logging level is set at WARNING or more, but can be lowered by calling **logging.disable()**,
 for example with the *logging.NOTSET* parameter to get DEBUG or more logging level.
 
 The **handle_interrupt_signals()** function calls the specified *handler_function* to process the SIGINT and SIGPIPE signals,
 usually to avoid an ugly trace dump to the console in case of interrupt (Control-C pressed or broken pipe).
 
 The **get_home_directory()** function returns the location of the user's home directory in a string
 depending on the operating system used (Unix, Windows).
 
+The **get_caching_directory()** function returns the location of a user writable directory for caching files in a string
+depending on the operating system used (Unix, Windows).
+The provided *name* will be the last directory part of this location.
+
 The **locate_directory()** function searches the specified *directory* in a variety of possible other directories,
 depending on the operating system used (Unix, Windows) and the fact that a package can be user or system installed.
 It is intended to be used when the directory can't be directly found, and returns a list of paths where the directory searched has been found.
 
 For example, if the argument is "/usr/local/etc/man.d", we'll search for "usr/local/etc/man.d", "local/etc/man.d", "etc/man.d" (more likely) and "man.d"
 in a list of user's local Python package directories
 ("$HOME/.local" on Unix, "$APPDATA/python", "$HOMEPATH/appdata/roaming/python", "$USERPROFILE/appdata/roaming/python" on Windows)
 and system wide Python package base directories (given by *sys.base_prefix*: "/usr/local" on Unix, "C:/Program Files/Python3x" on Windows).
 
+The **load_strings_from_file()** function returns a list of strings from the given *filename*,
+filtering out blank or commented lines, as well as end-of-line comments (with '#' being the comment character).
+
 ## ENVIRONMENT
-The following environment variables can be used to identify the user identity and home directory.
+The following environment variables can be used to identify the user identity and home directory,
+or find a caching directory.
 
-On Unix: *HOME*, *LOGNAME*, *USER*, *LNAME* and *USERNAME*.
+On Unix: *HOME*, *LNAME*, *LOGNAME*, *TMP*, *TMPDIR*, *USER* and *USERNAME*.
 
-On Windows: *APPDATA*, *HOME*, *HOMEPATH* and *USERPROFILE*.
+On Windows: *APPDATA*, *HOME*, *HOMEPATH*, *LOCALAPPDATA*, *TMP* and *USERPROFILE*.
 
 ## STANDARDS
 The **libpnu** library is not a standard UNIX one.
 
 It tries to follow the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide for [Python](https://www.python.org/) code.
 
 ## PORTABILITY
-To be tested under Windows.
+Tested OK under Windows.
 
 ## HISTORY
 This library was made for the [PNU project](https://github.com/HubTou/PNU).
 
 ## LICENSE
 It is available under the [3-clause BSD license](https://opensource.org/licenses/BSD-3-Clause).
```

### Comparing `pnu_libpnu-1.1.2/setup.cfg` & `pnu-libpnu-1.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
-name = pnu_libpnu
+name = pnu-libpnu
 description = Common utility functions for the PNU project
 long_description = file: README.md
 long_description_content_type = text/markdown
-version = 1.1.2
+version = 1.2.0
 license = BSD 3-Clause License
 license_files = License
 author = Hubert Tournier
 author_email = hubert.tournier@gmail.com
 url = https://github.com/HubTou/libpnu/
 project_urls = 
 	Bug Tracker = https://github.com/HubTou/libpnu/issues
@@ -26,14 +26,15 @@
 	Programming Language :: Python :: 3.4
 	Programming Language :: Python :: 3.5
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.3
```

### Comparing `pnu_libpnu-1.1.2/src/pnu_libpnu.egg-info/PKG-INFO` & `pnu-libpnu-1.2.0/src/pnu_libpnu.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pnu-libpnu
-Version: 1.1.2
+Version: 1.2.0
 Summary: Common utility functions for the PNU project
 Home-page: https://github.com/HubTou/libpnu/
 Author: Hubert Tournier
 Author-email: hubert.tournier@gmail.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/HubTou/libpnu/issues
 Keywords: pnu-project
@@ -21,21 +21,22 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.3
 Description-Content-Type: text/markdown
 License-File: License
 
 # Installation
-pip install [pnu-libpnu](https://pypi.org/project/pnu-libpnu/)
+This library will be installed as a dependency by other PNU utilities.
 
 # LIBPNU(3)
 
 ## NAME
 libpnu — Common utility functions for the PNU project
 
 ## SYNOPSIS
@@ -43,50 +44,62 @@
 
 *libpnu*.**initialize_debugging**(String *program_name*)
 
 *libpnu*.**handle_interrupt_signals**(Function *handler_function*)
 
 String *libpnu*.**get_home_directory**()
 
+String *libpnu*.**get_caching_directory**(String *name*)
+
 List *libpnu*.**locate_directory**(String *directory*)
 
+List *libpnu*.**load_strings_from_file**(String *filename*)
+
 ## DESCRIPTION
 The **initialize_debugging()** function sets up the Python logging module with a syslog style kind of console log using *program_name* as the program name.
 By default, the logging level is set at WARNING or more, but can be lowered by calling **logging.disable()**,
 for example with the *logging.NOTSET* parameter to get DEBUG or more logging level.
 
 The **handle_interrupt_signals()** function calls the specified *handler_function* to process the SIGINT and SIGPIPE signals,
 usually to avoid an ugly trace dump to the console in case of interrupt (Control-C pressed or broken pipe).
 
 The **get_home_directory()** function returns the location of the user's home directory in a string
 depending on the operating system used (Unix, Windows).
 
+The **get_caching_directory()** function returns the location of a user writable directory for caching files in a string
+depending on the operating system used (Unix, Windows).
+The provided *name* will be the last directory part of this location.
+
 The **locate_directory()** function searches the specified *directory* in a variety of possible other directories,
 depending on the operating system used (Unix, Windows) and the fact that a package can be user or system installed.
 It is intended to be used when the directory can't be directly found, and returns a list of paths where the directory searched has been found.
 
 For example, if the argument is "/usr/local/etc/man.d", we'll search for "usr/local/etc/man.d", "local/etc/man.d", "etc/man.d" (more likely) and "man.d"
 in a list of user's local Python package directories
 ("$HOME/.local" on Unix, "$APPDATA/python", "$HOMEPATH/appdata/roaming/python", "$USERPROFILE/appdata/roaming/python" on Windows)
 and system wide Python package base directories (given by *sys.base_prefix*: "/usr/local" on Unix, "C:/Program Files/Python3x" on Windows).
 
+The **load_strings_from_file()** function returns a list of strings from the given *filename*,
+filtering out blank or commented lines, as well as end-of-line comments (with '#' being the comment character).
+
 ## ENVIRONMENT
-The following environment variables can be used to identify the user identity and home directory.
+The following environment variables can be used to identify the user identity and home directory,
+or find a caching directory.
 
-On Unix: *HOME*, *LOGNAME*, *USER*, *LNAME* and *USERNAME*.
+On Unix: *HOME*, *LNAME*, *LOGNAME*, *TMP*, *TMPDIR*, *USER* and *USERNAME*.
 
-On Windows: *APPDATA*, *HOME*, *HOMEPATH* and *USERPROFILE*.
+On Windows: *APPDATA*, *HOME*, *HOMEPATH*, *LOCALAPPDATA*, *TMP* and *USERPROFILE*.
 
 ## STANDARDS
 The **libpnu** library is not a standard UNIX one.
 
 It tries to follow the [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide for [Python](https://www.python.org/) code.
 
 ## PORTABILITY
-To be tested under Windows.
+Tested OK under Windows.
 
 ## HISTORY
 This library was made for the [PNU project](https://github.com/HubTou/PNU).
 
 ## LICENSE
 It is available under the [3-clause BSD license](https://opensource.org/licenses/BSD-3-Clause).
```

