# Comparing `tmp/jpylib-jyrgenn-2023.214.1627.tar.gz` & `tmp/jpylib-jyrgenn-2023.508.846.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jpylib-jyrgenn-2023.214.1627.tar", last modified: Tue Feb 14 15:27:25 2023, max compression
+gzip compressed data, was "jpylib-jyrgenn-2023.508.846.tar", last modified: Mon May  8 06:46:35 2023, max compression
```

## Comparing `jpylib-jyrgenn-2023.214.1627.tar` & `jpylib-jyrgenn-2023.508.846.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 ni         (501) staff       (50)        0 2023-02-14 15:27:25.446481 jpylib-jyrgenn-2023.214.1627/
--rw-r--r--   0 ni         (501) staff       (50)     1068 2023-02-14 15:27:25.446481 jpylib-jyrgenn-2023.214.1627/PKG-INFO
--rw-r--r--   0 ni         (501) staff       (50)      516 2022-08-12 14:43:01.000000 jpylib-jyrgenn-2023.214.1627/README.md
-drwxr-xr-x   0 ni         (501) staff       (50)        0 2023-02-14 15:27:25.446481 jpylib-jyrgenn-2023.214.1627/jpylib/
--rwxr-xr-x   0 ni         (501) staff       (50)     2578 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/__init__.py
--rwxr-xr-x   0 ni         (501) staff       (50)    12109 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/alerts.py
--rwxr-xr-x   0 ni         (501) staff       (50)     1868 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/assorted.py
--rwxr-xr-x   0 ni         (501) staff       (50)     4537 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/capture.py
--rwxr-xr-x   0 ni         (501) staff       (50)     3329 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/config.py
--rwxr-xr-x   0 ni         (501) staff       (50)      508 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/fntrace.py
--rw-r--r--   0 ni         (501) staff       (50)     4640 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/iohelper.py
--rwxr-xr-x   0 ni         (501) staff       (50)     5860 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/kvs.py
--rw-r--r--   0 ni         (501) staff       (50)     2275 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/multiset.py
--rwxr-xr-x   0 ni         (501) staff       (50)     2720 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/namespace.py
--rw-r--r--   0 ni         (501) staff       (50)     1756 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/numeric.py
--rwxr-xr-x   0 ni         (501) staff       (50)    12225 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/options.py
--rwxr-xr-x   0 ni         (501) staff       (50)     2803 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/process.py
--rwxr-xr-x   0 ni         (501) staff       (50)    10543 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/secrets.py
--rwxr-xr-x   0 ni         (501) staff       (50)     1359 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/sighandler.py
--rw-r--r--   0 ni         (501) staff       (50)      454 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/singleton.py
--rwxr-xr-x   0 ni         (501) staff       (50)     1569 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/stringreader.py
--rwxr-xr-x   0 ni         (501) staff       (50)    10668 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/table.py
--rwxr-xr-x   0 ni         (501) staff       (50)     2988 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/table_templates.py
--rwxr-xr-x   0 ni         (501) staff       (50)     1179 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/terminal.py
--rwxr-xr-x   0 ni         (501) staff       (50)      695 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib/time.py
-drwxr-xr-x   0 ni         (501) staff       (50)        0 2023-02-14 15:27:25.446481 jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/
--rw-r--r--   0 ni         (501) staff       (50)     1068 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/PKG-INFO
--rw-r--r--   0 ni         (501) staff       (50)      562 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/SOURCES.txt
--rw-r--r--   0 ni         (501) staff       (50)        1 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/dependency_links.txt
--rw-r--r--   0 ni         (501) staff       (50)        7 2023-02-14 15:27:25.000000 jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/top_level.txt
--rw-r--r--   0 ni         (501) staff       (50)       38 2023-02-14 15:27:25.446481 jpylib-jyrgenn-2023.214.1627/setup.cfg
--rwxr-xr-x   0 ni         (501) staff       (50)     1067 2022-08-12 14:43:01.000000 jpylib-jyrgenn-2023.214.1627/setup.py
+drwxr-xr-x   0 ni         (501) staff       (20)        0 2023-05-08 06:46:35.465014 jpylib-jyrgenn-2023.508.846/
+-rw-r--r--   0 ni         (501) staff       (20)     1028 2023-05-08 06:46:35.464896 jpylib-jyrgenn-2023.508.846/PKG-INFO
+-rw-r--r--   0 ni         (501) staff       (20)      516 2022-03-11 11:18:51.000000 jpylib-jyrgenn-2023.508.846/README.md
+drwxr-xr-x   0 ni         (501) staff       (20)        0 2023-05-08 06:46:35.464128 jpylib-jyrgenn-2023.508.846/jpylib/
+-rwxr-xr-x   0 ni         (501) staff       (20)     2577 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/__init__.py
+-rwxr-xr-x   0 ni         (501) staff       (20)    12304 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/alerts.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     1868 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/assorted.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     4537 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/capture.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     3329 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/config.py
+-rwxr-xr-x   0 ni         (501) staff       (20)      508 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/fntrace.py
+-rw-r--r--   0 ni         (501) staff       (20)     4640 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/iohelper.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     5860 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/kvs.py
+-rw-r--r--   0 ni         (501) staff       (20)     2275 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/multiset.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     2720 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/namespace.py
+-rw-r--r--   0 ni         (501) staff       (20)     1756 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/numeric.py
+-rwxr-xr-x   0 ni         (501) staff       (20)    12320 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/options.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     2803 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/process.py
+-rwxr-xr-x   0 ni         (501) staff       (20)    10543 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/secrets.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     1359 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/sighandler.py
+-rw-r--r--   0 ni         (501) staff       (20)      454 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/singleton.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     1569 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/stringreader.py
+-rwxr-xr-x   0 ni         (501) staff       (20)    10669 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/table.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     2988 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/table_templates.py
+-rwxr-xr-x   0 ni         (501) staff       (20)     1179 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/terminal.py
+-rwxr-xr-x   0 ni         (501) staff       (20)      695 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib/time.py
+drwxr-xr-x   0 ni         (501) staff       (20)        0 2023-05-08 06:46:35.464742 jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/
+-rw-r--r--   0 ni         (501) staff       (20)     1028 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/PKG-INFO
+-rw-r--r--   0 ni         (501) staff       (20)      562 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/SOURCES.txt
+-rw-r--r--   0 ni         (501) staff       (20)        1 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/dependency_links.txt
+-rw-r--r--   0 ni         (501) staff       (20)        7 2023-05-08 06:46:35.000000 jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/top_level.txt
+-rw-r--r--   0 ni         (501) staff       (20)       38 2023-05-08 06:46:35.465050 jpylib-jyrgenn-2023.508.846/setup.cfg
+-rwxr-xr-x   0 ni         (501) staff       (20)     1067 2022-03-11 11:19:38.000000 jpylib-jyrgenn-2023.508.846/setup.py
```

### Comparing `jpylib-jyrgenn-2023.214.1627/PKG-INFO` & `jpylib-jyrgenn-2023.508.846/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: jpylib-jyrgenn
-Version: 2023.214.1627
+Version: 2023.508.846
 Summary: Utilities library with several more or less independent components
 Home-page: https://git.w21.org/ni/jpylib/
 Author: Juergen Nickelsen
 Author-email: ni@w21.org
-License: UNKNOWN
-Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.214.1627/doc/jpylib.md
+Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.508.846/doc/jpylib.md
 Project-URL: Source, https://git.w21.org/ni/jpylib/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Utilities library with several more or less independent components
 
 This library is mainly intended for myself, so I can access it from
 anywhere. But anyone else is welcome to have a look. Documentation
 is still lacking, I know, but that shall change. Testing is better.
 
 The full documentation (what already exists of it) for this version
 is at
-<https://git.w21.org/ni/jpylib/-/blob/v2023.214.1627/doc/jpylib.md>
+<https://git.w21.org/ni/jpylib/-/blob/v2023.508.846/doc/jpylib.md>
 
 [ni@w21.org 2022-03-11]
-
-
```

### Comparing `jpylib-jyrgenn-2023.214.1627/README.md` & `jpylib-jyrgenn-2023.508.846/README.md`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/__init__.py` & `jpylib-jyrgenn-2023.508.846/jpylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
      avg_midrange, remove_outliers
 from .iohelper import all_input_lines, read_items, read_mapping
 from .time import isotime, isotime_ms, iso_time, iso_time_ms, iso_time_us
 from .table import format_table
 from .singleton import Singleton
 from .multiset import Multiset
 
-version = "2023.214.1627"
+version = "2023.508.846"
 """The version of the `jpylib` package."""
 
 program = os.path.basename(sys.argv[0])
 """The name of the current program without its directory path."""
 
 real_home = pwd.getpwuid(os.getuid()).pw_dir
 """The home directory of the current user as defined for its user id."""
```

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/alerts.py` & `jpylib-jyrgenn-2023.508.846/jpylib/alerts.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     locals()[name] = i
 
 # the module configuration; will be initialised in alert_init()
 cfg = None
 
 def alert_config(*, decoration=None, fd=None, level=None, program=None,
                  syslog_facility=None, syslog_prio=None, reset_defaults=None,
-                 timestamps=None):
+                 timestamps=None, fatal_label="Fatal,"):
     """Customise the alerts configuration with the given values.
 
     If `reset_defaults` is true, reset everything to the specified or
     default values.
     """
     global cfg
     if not any(locals().values()) or reset_defaults:
@@ -147,14 +147,17 @@
             
             # maximum alert level
             max_level=len(alert_levels)-1,
 
             # print timestamps with messages
             timestamps=False,
 
+            # print "Fatal" label for fatal errors
+            fatal_label=fatal_label,
+
             # had any errors yet?
             had_errors=False,
         )
     del reset_defaults
     for var, value in locals().items():
         if value is not None:
             cfg.set(var, value)
@@ -317,15 +320,18 @@
     `template` is the format template, `args` are its arguments.
     """
     err(template.format(*args))
 errorf = errf
 
 def fatal(*msgs, exit_status=1):
     """Print `L_ERROR` level output and end the program with `exit_status`."""
-    alert_if_level(L_ERROR, "Fatal,", *msgs)
+    if cfg.fatal_label:
+        alert_if_level(L_ERROR, cfg.fatal_label, *msgs)
+    else:
+        alert_if_level(L_ERROR, *msgs)
     sys.exit(exit_status)
 
 def fatalf(template, *args, exit_status=1):
     """Print `L_ERROR` level output and end the program with `exit_status`.
 
     `template` is the format template, `args` are its arguments.
     """
```

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/assorted.py` & `jpylib-jyrgenn-2023.508.846/jpylib/assorted.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/capture.py` & `jpylib-jyrgenn-2023.508.846/jpylib/capture.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/config.py` & `jpylib-jyrgenn-2023.508.846/jpylib/config.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/iohelper.py` & `jpylib-jyrgenn-2023.508.846/jpylib/iohelper.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/kvs.py` & `jpylib-jyrgenn-2023.508.846/jpylib/kvs.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/multiset.py` & `jpylib-jyrgenn-2023.508.846/jpylib/multiset.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/namespace.py` & `jpylib-jyrgenn-2023.508.846/jpylib/namespace.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/numeric.py` & `jpylib-jyrgenn-2023.508.846/jpylib/numeric.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/options.py` & `jpylib-jyrgenn-2023.508.846/jpylib/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,16 +82,19 @@
             self._max = None if inf else max
             self._arguments = " ".join(self._arguments)
 
 
     def _parse(self):
         while self._args and self._args[0].startswith("-"):
             arg = self._args.pop(0)
-            if arg == "--": break
+            if arg == "-":
+                self._args.insert(0, arg)
+                break
             if arg.startswith("--"):
+                if arg == "--": break
                 self._have_opt(arg[2:])
             else:
                 arg = arg[1:]
                 while arg:
                     arg = self._have_opt(arg[0], arg[1:])
         if self._min is not None and len(self._args) < self._min:
             raise ArgumentError(ErrorMinarg, self._min)
```

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/process.py` & `jpylib-jyrgenn-2023.508.846/jpylib/process.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/secrets.py` & `jpylib-jyrgenn-2023.508.846/jpylib/secrets.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/sighandler.py` & `jpylib-jyrgenn-2023.508.846/jpylib/sighandler.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/stringreader.py` & `jpylib-jyrgenn-2023.508.846/jpylib/stringreader.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/table.py` & `jpylib-jyrgenn-2023.508.846/jpylib/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         * hl_cross[2]:   header separator line crossing, first and others
         * nl_cross[2]:   normal separator line crossing, first and others
         * cell_pad[2]:   minimum cell padding, left and right (integers)
         * pad_char:      padding character
         * template:      a template 7 x 7 drawing describing the table
         * align:         alignment descriptor string, 1 char per column, l/r/c;
                          may be sequence of 2 for first and following rows;
-                         asterisk at the end means default for folloing columns
+                         asterisk at the end means default for following columns
                          is the character in front of the asterisk
         * data:          the data to format, as a sequence of rows, which are
                          sequences of columns (the data items)
         * rstrip:        strip trailing blanks off output lines
         * intend:        a string to lead each output line
 
         Parameters are first taken from the template, if any, and
```

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/table_templates.py` & `jpylib-jyrgenn-2023.508.846/jpylib/table_templates.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/terminal.py` & `jpylib-jyrgenn-2023.508.846/jpylib/terminal.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib/time.py` & `jpylib-jyrgenn-2023.508.846/jpylib/time.py`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/PKG-INFO` & `jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 Metadata-Version: 2.1
 Name: jpylib-jyrgenn
-Version: 2023.214.1627
+Version: 2023.508.846
 Summary: Utilities library with several more or less independent components
 Home-page: https://git.w21.org/ni/jpylib/
 Author: Juergen Nickelsen
 Author-email: ni@w21.org
-License: UNKNOWN
-Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.214.1627/doc/jpylib.md
+Project-URL: Documentation, https://git.w21.org/ni/jpylib//-/blob/v2023.508.846/doc/jpylib.md
 Project-URL: Source, https://git.w21.org/ni/jpylib/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Utilities library with several more or less independent components
 
 This library is mainly intended for myself, so I can access it from
 anywhere. But anyone else is welcome to have a look. Documentation
 is still lacking, I know, but that shall change. Testing is better.
 
 The full documentation (what already exists of it) for this version
 is at
-<https://git.w21.org/ni/jpylib/-/blob/v2023.214.1627/doc/jpylib.md>
+<https://git.w21.org/ni/jpylib/-/blob/v2023.508.846/doc/jpylib.md>
 
 [ni@w21.org 2022-03-11]
-
-
```

### Comparing `jpylib-jyrgenn-2023.214.1627/jpylib_jyrgenn.egg-info/SOURCES.txt` & `jpylib-jyrgenn-2023.508.846/jpylib_jyrgenn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jpylib-jyrgenn-2023.214.1627/setup.py` & `jpylib-jyrgenn-2023.508.846/setup.py`

 * *Files identical despite different names*

