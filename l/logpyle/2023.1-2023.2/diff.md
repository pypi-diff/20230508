# Comparing `tmp/logpyle-2023.1.tar.gz` & `tmp/logpyle-2023.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logpyle-2023.1.tar", last modified: Tue Feb 14 19:39:23 2023, max compression
+gzip compressed data, was "logpyle-2023.2.tar", last modified: Mon May  8 21:07:15 2023, max compression
```

## Comparing `logpyle-2023.1.tar` & `logpyle-2023.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-02-14 19:39:23.257894 logpyle-2023.1/
--rw-r--r--   0 mdiener    (501) staff       (20)     1212 2023-01-24 03:48:22.000000 logpyle-2023.1/LICENSE
--rw-r--r--   0 mdiener    (501) staff       (20)     1703 2023-02-14 19:39:23.257962 logpyle-2023.1/PKG-INFO
--rw-r--r--   0 mdiener    (501) staff       (20)      617 2023-01-24 03:48:22.000000 logpyle-2023.1/README.md
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-02-14 19:39:23.255952 logpyle-2023.1/bin/
--rwxr-xr-x   0 mdiener    (501) staff       (20)     8934 2023-01-24 03:48:22.000000 logpyle-2023.1/bin/logtool
--rwxr-xr-x   0 mdiener    (501) staff       (20)     1410 2023-01-24 03:48:22.000000 logpyle-2023.1/bin/runalyzer
--rwxr-xr-x   0 mdiener    (501) staff       (20)    14149 2023-01-24 03:48:22.000000 logpyle-2023.1/bin/runalyzer-gather
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-02-14 19:39:23.257057 logpyle-2023.1/logpyle/
--rw-r--r--   0 mdiener    (501) staff       (20)    49326 2023-02-14 19:31:03.000000 logpyle-2023.1/logpyle/__init__.py
--rw-r--r--   0 mdiener    (501) staff       (20)        0 2023-01-24 03:48:22.000000 logpyle-2023.1/logpyle/py.typed
--rw-r--r--   0 mdiener    (501) staff       (20)    13823 2023-01-24 03:48:22.000000 logpyle-2023.1/logpyle/runalyzer.py
--rw-r--r--   0 mdiener    (501) staff       (20)      106 2023-02-14 19:31:50.000000 logpyle-2023.1/logpyle/version.py
-drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-02-14 19:39:23.257779 logpyle-2023.1/logpyle.egg-info/
--rw-r--r--   0 mdiener    (501) staff       (20)     1703 2023-02-14 19:39:23.000000 logpyle-2023.1/logpyle.egg-info/PKG-INFO
--rw-r--r--   0 mdiener    (501) staff       (20)      314 2023-02-14 19:39:23.000000 logpyle-2023.1/logpyle.egg-info/SOURCES.txt
--rw-r--r--   0 mdiener    (501) staff       (20)        1 2023-02-14 19:39:23.000000 logpyle-2023.1/logpyle.egg-info/dependency_links.txt
--rw-r--r--   0 mdiener    (501) staff       (20)       25 2023-02-14 19:39:23.000000 logpyle-2023.1/logpyle.egg-info/requires.txt
--rw-r--r--   0 mdiener    (501) staff       (20)        8 2023-02-14 19:39:23.000000 logpyle-2023.1/logpyle.egg-info/top_level.txt
--rw-r--r--   0 mdiener    (501) staff       (20)      393 2023-02-14 19:39:23.258298 logpyle-2023.1/setup.cfg
--rw-r--r--   0 mdiener    (501) staff       (20)     1832 2023-01-24 03:48:22.000000 logpyle-2023.1/setup.py
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-08 21:07:15.480122 logpyle-2023.2/
+-rw-r--r--   0 mdiener    (501) staff       (20)     1212 2023-03-27 22:23:58.000000 logpyle-2023.2/LICENSE
+-rw-r--r--   0 mdiener    (501) staff       (20)     1653 2023-05-08 21:07:15.480183 logpyle-2023.2/PKG-INFO
+-rw-r--r--   0 mdiener    (501) staff       (20)      617 2023-03-27 22:23:58.000000 logpyle-2023.2/README.md
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-08 21:07:15.478249 logpyle-2023.2/bin/
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     9253 2023-04-18 21:26:43.000000 logpyle-2023.2/bin/logtool
+-rwxr-xr-x   0 mdiener    (501) staff       (20)     1730 2023-05-08 20:44:06.000000 logpyle-2023.2/bin/runalyzer
+-rwxr-xr-x   0 mdiener    (501) staff       (20)    13649 2023-05-08 19:53:56.000000 logpyle-2023.2/bin/runalyzer-gather
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-08 21:07:15.479357 logpyle-2023.2/logpyle/
+-rw-r--r--   0 mdiener    (501) staff       (20)    55409 2023-05-08 20:44:06.000000 logpyle-2023.2/logpyle/__init__.py
+-rw-r--r--   0 mdiener    (501) staff       (20)        0 2023-03-27 22:23:58.000000 logpyle-2023.2/logpyle/py.typed
+-rw-r--r--   0 mdiener    (501) staff       (20)    15519 2023-05-08 19:53:56.000000 logpyle-2023.2/logpyle/runalyzer.py
+-rw-r--r--   0 mdiener    (501) staff       (20)      106 2023-05-08 21:06:00.000000 logpyle-2023.2/logpyle/version.py
+drwxr-xr-x   0 mdiener    (501) staff       (20)        0 2023-05-08 21:07:15.480015 logpyle-2023.2/logpyle.egg-info/
+-rw-r--r--   0 mdiener    (501) staff       (20)     1653 2023-05-08 21:07:15.000000 logpyle-2023.2/logpyle.egg-info/PKG-INFO
+-rw-r--r--   0 mdiener    (501) staff       (20)      314 2023-05-08 21:07:15.000000 logpyle-2023.2/logpyle.egg-info/SOURCES.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)        1 2023-05-08 21:07:15.000000 logpyle-2023.2/logpyle.egg-info/dependency_links.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)       25 2023-05-08 21:07:15.000000 logpyle-2023.2/logpyle.egg-info/requires.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)        8 2023-05-08 21:07:15.000000 logpyle-2023.2/logpyle.egg-info/top_level.txt
+-rw-r--r--   0 mdiener    (501) staff       (20)      393 2023-05-08 21:07:15.480436 logpyle-2023.2/setup.cfg
+-rw-r--r--   0 mdiener    (501) staff       (20)     1781 2023-04-18 21:26:43.000000 logpyle-2023.2/setup.py
```

### Comparing `logpyle-2023.1/LICENSE` & `logpyle-2023.2/LICENSE`

 * *Files identical despite different names*

### Comparing `logpyle-2023.1/PKG-INFO` & `logpyle-2023.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: logpyle
-Version: 2023.1
+Version: 2023.2
 Summary: Time series logging for Python
 Home-page: https://github.com/illinois-ceesd/logpyle
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logpyle: Time Series Logging (not just) for Simulation
 
 [![CI](https://github.com/illinois-ceesd/logpyle/workflows/CI/badge.svg)](https://github.com/illinois-ceesd/logpyle/actions?query=workflow%3ACI+branch%3Amain)
 [![Documentation Status](https://readthedocs.org/projects/logpyle/badge/?version=latest)](https://logpyle.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `logpyle-2023.1/README.md` & `logpyle-2023.2/README.md`

 * *Files identical despite different names*

### Comparing `logpyle-2023.1/bin/logtool` & `logpyle-2023.2/bin/logtool`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #! /usr/bin/env python
 
-def main():
-    from logpyle import LogManager
+from typing import Optional, Tuple
+
+
+def main() -> None:
     import sys
     from optparse import OptionParser
 
+    from logpyle import LogManager
+
     description = """Operate on data gathered during code runs.
 FILE is a log saved from a code run. COMMANDS may be one of the
 following:
 "list" to list the available time-series and constants,
 "plot expr_x,expr_y" to plot a graph,
 "datafile outfile expr_x,expr_y" to write out a data file.
 "table variable" to print the full data table for a time series variable.
@@ -62,36 +66,40 @@
 
     did_plot = False
     saveplot_filename = None
     print_plot = False
 
     legend_prefix = ""
 
-    from pytools import cartesian_product, Record
+    from dataclasses import dataclass
+    from itertools import product
 
-    class PlotStyle(Record):
-        pass
+    @dataclass(frozen=True)
+    class PlotStyle:
+        dashes: Tuple[int, ...]
+        color: str
 
     styles = [
             PlotStyle(dashes=dashes, color=color)
-            for dashes, color in cartesian_product(
+            for dashes, color in product(
                 [(), (12, 2), (4, 2),  (2, 2), (2, 8)],
                 ["blue", "green", "red", "magenta", "cyan"],
                 )]
 
-    def check_no_file():
+    def check_no_file() -> None:
         if logmgr is None:
             raise RuntimeError("no file loaded")
 
     next_legend = None
 
     while args:
         cmd = args.pop(0)
         if cmd == "list":
             check_no_file()
+            assert logmgr
 
             print("Time series")
             print("-----------")
 
             items = list(logmgr.quantity_data.items())
             items.sort(key=lambda item: item[0])
 
@@ -114,18 +122,19 @@
             else:
                 col0_len = 0
 
             for key, value in items:
                 print("{}\t{}".format(key.ljust(col0_len), str(value)))
         elif cmd == "plot":
             check_no_file()
+            assert logmgr
 
             expr_x, expr_y = args.pop(0).split(",")
 
-            from matplotlib.pyplot import xlabel, ylabel, plot
+            from matplotlib.pyplot import plot, xlabel, ylabel
             (data_x, descr_x, unit_x), (data_y, descr_y, unit_y) = \
                     logmgr.get_plot_data(expr_x, expr_y,
                             options.start_step, options.end_step)
 
             if options.label_x:
                 xlabel(options.label_x)
             else:
@@ -158,28 +167,31 @@
                     dashes=style.dashes, color=style.color,
                     hold=True,  **kwargs)
 
             did_plot = True
             next_legend = None
         elif cmd == "warnings":
             check_no_file()
+            assert logmgr
             print(logmgr.get_warnings())
 
         elif cmd == "datafile":
             check_no_file()
+            assert logmgr
 
             expr_x, expr_y = args.pop(0).split(",")
 
             logmgr.write_datafile(args.pop(0), expr_x, expr_y)
         elif cmd == "prefix":
             legend_prefix = args.pop(0)
         elif cmd == "next_legend":
             next_legend = args.pop(0)
         elif cmd == "table":
             check_no_file()
+            assert logmgr
 
             descrs, units, data = logmgr.get_joint_dataset(args.pop(0).split(","))
             if options.start_step is not None:
                 data = [(step, tup) for step, tup in data
                         if options.start_step <= step]
             if options.end_step is not None:
                 data = [(step, tup) for step, tup in data
@@ -195,31 +207,32 @@
             print(tbl)
         elif cmd == "saveplot":
             saveplot_filename = args.pop(0)
         elif cmd == "print":
             print_plot = True
         else:
             # not a known command, interpret as file name
-            from os import access, R_OK
+            from os import R_OK, access
             if access(cmd, R_OK):
                 logmgr = LogManager(cmd, "r")
             else:
                 raise OSError("file '%s' not found" % cmd)
 
     if did_plot:
-        from matplotlib.pyplot import show, title, legend, axis, grid, rc, savefig
+        from matplotlib.pyplot import (axis, grid, legend, rc, savefig, show,
+                                       title)
         if options.legend_expr or options.legend_descr:
             if options.small_legend:
                 from matplotlib.font_manager import FontProperties
                 legend(borderpad=0.04, prop=FontProperties(size=8), loc="best",
                         labelspacing=0)
             else:
                 legend(loc="best")
 
-        def float_or_none(str):
+        def float_or_none(str: str) -> Optional[float]:
             if str == "*":
                 return None
             else:
                 return float(str)
 
         xmin, xmax, ymin, ymax = axis()
         if options.scale_x:
@@ -241,16 +254,16 @@
 
         if options.grid:
             grid()
 
         title(options.title)
 
         if print_plot:
-            from tempfile import gettempprefix, gettempdir
             import os.path
+            from tempfile import gettempdir, gettempprefix
             tmpname = os.path.join(gettempdir(), gettempprefix()+"logtoolprint.ps")
             savefig(tmpname, orientation="landscape", papertype="letter")
 
             from os import system, unlink
             system("lp %s" % tmpname)
 
             unlink(tmpname)
```

### Comparing `logpyle-2023.1/bin/runalyzer` & `logpyle-2023.2/bin/runalyzer`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 #! /usr/bin/env python
 
 
-def main():
-    import sys
+def main() -> None:
     import argparse
+    import sys
 
     parser = argparse.ArgumentParser(description="Analyze a logpyle database.")
     parser.add_argument("-m", "--mangle", action="store_true",
-            help="whether to try and mangle SQL queries")
+            help="(ignored)")
+    parser.add_argument("-n", "--nomangle", action="store_true",
+            help="disable mangling of SQL queries")
     parser.add_argument("-c", "--commands", action="store",
             help="commands to execute")
     parser.add_argument("dbfile", help="database file to read")
     parser.add_argument("scriptfile", nargs="?", help="script file to read")
     args = parser.parse_args()
 
-    from logpyle.runalyzer import make_wrapped_db, make_runalyzer_symbols
+    from logpyle.runalyzer import make_runalyzer_symbols, make_wrapped_db
+
+    if args.mangle:
+        from warnings import warn
+        warn("The -m/--mangle option is deprecated, mangling is enabled by "
+             "default. Disable mangling with -n/--nomangle.")
+
+    do_mangle = not args.nomangle
 
     if args.scriptfile:
-        db = make_wrapped_db(args.dbfile, mangle=args.mangle, interactive=False)
+        db = make_wrapped_db(args.dbfile, mangle=do_mangle, interactive=False)
         exec(compile(open(args.scriptfile).read(), args.scriptfile, "exec"),
                 make_runalyzer_symbols(db))
     elif args.commands:
-        db = make_wrapped_db(args.dbfile, mangle=args.mangle, interactive=False)
+        db = make_wrapped_db(args.dbfile, mangle=do_mangle, interactive=False)
         exec(compile(args.commands, "--commands", "exec"),
                 make_runalyzer_symbols(db))
     else:
-        db = make_wrapped_db(args.dbfile, mangle=args.mangle, interactive=True)
+        db = make_wrapped_db(args.dbfile, mangle=do_mangle, interactive=True)
         from logpyle.runalyzer import RunalyzerConsole
         cons = RunalyzerConsole(db)
         cons.interact("Runalyzer running on Python %s\n"
                 "Run .help to see help for 'magic' commands" % sys.version)
 
 
 if __name__ == "__main__":
```

### Comparing `logpyle-2023.1/bin/runalyzer-gather` & `logpyle-2023.2/bin/runalyzer-gather`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 #! /usr/bin/env python
 
 import re
 
-
 bool_feat_re = re.compile(r"^([a-z]+)(True|False)$")
 int_feat_re = re.compile(r"^([a-z]+)([0-9]+)$")
 real_feat_re = re.compile(r"^([a-z]+)([0-9]+\.?[0-9]*)$")
 str_feat_re = re.compile(r"^([a-z]+)([A-Z][A-Za-z_0-9]+)$")
 
+from sqlite3 import Connection
+from typing import Any, Dict, List, Optional, Tuple, Union, cast
+
+from pytools.datatable import DataTable
+
+from logpyle import LogManager
 
 sqlite_keywords = """
     abort action add after all alter analyze and as asc attach
     autoincrement before begin between by cascade case cast check
     collate column commit conflict constraint create cross current_date
     current_time current_timestamp database default deferrable deferred
     delete desc detach distinct drop each else end escape except
@@ -21,15 +26,16 @@
     natural no not notnull null of offset on or order outer plan pragma
     primary query raise references regexp reindex release rename
     replace restrict right rollback row savepoint select set table temp
     temporary then to transaction trigger union unique update using
     vacuum values view virtual when where""".split()
 
 
-def parse_dir_feature(feat, number):
+def parse_dir_feature(feat: str, number: int) \
+                        -> Tuple[Union[str, Any], str, Union[str, Any]]:
     bool_match = bool_feat_re.match(feat)
     if bool_match is not None:
         return (bool_match.group(1), "integer", int(bool_match.group(2) == "True"))
     int_match = int_feat_re.match(feat)
     if int_match is not None:
         return (int_match.group(1), "integer", float(int_match.group(2)))
     real_match = real_feat_re.match(feat)
@@ -37,15 +43,15 @@
         return (real_match.group(1), "real", float(real_match.group(2)))
     str_match = str_feat_re.match(feat)
     if str_match is not None:
         return (str_match.group(1), "text", str_match.group(2))
     return ("dirfeat%d" % number, "text", feat)
 
 
-def larger_sql_type(type_a, type_b):
+def larger_sql_type(type_a: Optional[str], type_b: Optional[str]) -> Optional[str]:
     assert type_a in [None, "text", "real", "integer"]
     assert type_b in [None, "text", "real", "integer"]
 
     if type_a is None:
         return type_b
     if type_b is None:
         return type_a
@@ -53,28 +59,30 @@
         return "text"
     if "real" in [type_a, type_b]:
         return "real"
     assert type_a == type_b == "integer"
     return "integer"
 
 
-def sql_type_and_value(value):
+def sql_type_and_value(value: Any) \
+                        -> Tuple[Optional[str], Union[int, float, str, None]]:
     if value is None:
         return None, None
     elif isinstance(value, bool):
         return "integer", int(value)
     elif isinstance(value, int):
         return "integer", value
     elif isinstance(value, float):
         return "real", value
     else:
         return "text", str(value)
 
 
-def sql_type_and_value_from_str(value):
+def sql_type_and_value_from_str(value: str) \
+                        -> Tuple[Optional[str], Union[int, float, str, None]]:
     if value == "None":
         return None, None
     elif value in ["True", "False"]:
         return "integer", value == "True"
     else:
         try:
             return "integer", int(value)
@@ -84,15 +92,16 @@
             return "real", float(value)
         except ValueError:
             pass
         return "text", str(value)
 
 
 class FeatureGatherer:
-    def __init__(self, features_from_dir=False, features_file=None):
+    def __init__(self, features_from_dir: bool = False,
+                 features_file: Optional[str] = None) -> None:
         self.features_from_dir = features_from_dir
 
         self.dir_to_features = {}
         if features_file is not None:
             for line in open(features_file).readlines():
                 colon_idx = line.find(":")
                 assert colon_idx != -1
@@ -103,15 +112,15 @@
                     equal_idx = entry.find("=")
                     assert equal_idx != -1
                     features.append((entry[:equal_idx],)
                             + sql_type_and_value_from_str(entry[equal_idx+1:]))
 
                 self.dir_to_features[line[:colon_idx]] = features
 
-    def get_db_features(self, dbname, logmgr):
+    def get_db_features(self, dbname: str, logmgr: LogManager) -> List[Any]:
         from os.path import dirname
         dn = dirname(dbname)
 
         features = self.dir_to_features.get(dn, [])[:]
 
         if self.features_from_dir:
             features.extend(parse_dir_feature(feat, i)
@@ -119,66 +128,67 @@
 
         for name, value in logmgr.constants.items():
             features.append((name,) + sql_type_and_value(value))
 
         return features
 
 
-def scan(fg, dbnames, progress=True):
-    features = {}
+def scan(fg: FeatureGatherer, dbnames: List[str], progress: bool = True) \
+            -> Tuple[Dict[str, Any], Dict[str, int]]:
+    features: Dict[str, Any] = {}
     dbname_to_run_id = {}
-    uid_to_run_id = {}
+    uid_to_run_id: Dict[str, int] = {}
     next_run_id = 1
 
     from pytools import ProgressBar
     if progress:
-        pb = ProgressBar("Scanning...", len(dbnames))
+        pb = ProgressBar("Scanning...",  # type: ignore[no-untyped-call]
+                         len(dbnames))
 
     for dbname in dbnames:
-        from logpyle import LogManager
         try:
             logmgr = LogManager(dbname, "r")
         except Exception:
             print("Trouble with file '%s'" % dbname)
             raise
 
-        unique_run_id = logmgr.constants.get("unique_run_id")
+        unique_run_id = cast(str, logmgr.constants.get("unique_run_id"))
         run_id = uid_to_run_id.get(unique_run_id)
 
         if run_id is None:
             run_id = next_run_id
             next_run_id += 1
 
             if unique_run_id is not None:
                 uid_to_run_id[unique_run_id] = run_id
 
         dbname_to_run_id[dbname] = run_id
 
         if progress:
-            pb.progress()
+            pb.progress()  # type: ignore[no-untyped-call]
 
         for fname, ftype, fvalue in fg.get_db_features(dbname, logmgr):
             if fname in features:
                 features[fname] = larger_sql_type(ftype, features[fname])
             else:
                 if ftype is None:
                     ftype = "text"
                 features[fname] = ftype
 
         logmgr.close()
 
     if progress:
-        pb.finished()
+        pb.finished()  # type: ignore[no-untyped-call]
 
     return features, dbname_to_run_id
 
 
-def make_name_map(map_str):
+def make_name_map(map_str: str) -> Dict[str, str]:
     import re
-    result = {}
+    result: Dict[str, str] = {}
 
     if not map_str:
         return result
 
     map_re = re.compile(r"^([a-z_A-Z0-9]+)=([a-z_A-Z0-9]+)$")
     for fmap_entry in map_str.split(","):
         match = map_re.match(fmap_entry)
@@ -186,86 +196,29 @@
             raise RuntimeError(
                     "Arguments to -m should have the form F1=FNAME1,F2=FNAME2,...")
         result[match.group(1)] = match.group(2)
 
     return result
 
 
-def transfer_data_table(db_conn, tbl_name, data_table):
-    db_conn.executemany("insert into %s (%s) values (%s)" %
-            (tbl_name,
-                ", ".join(data_table.column_names),
-                ", ".join("?" * len(data_table.column_names))),
-            data_table.data)
-
-
-def gather_single_file(outfile, infiles):
-    from pytools import ProgressBar
-    pb = ProgressBar("Importing...", len(infiles))
-
-    import sqlite3
-    db_conn = sqlite3.connect(outfile)
-
-    from logpyle import _set_up_schema
-    _set_up_schema(db_conn)
-
-    from pickle import dumps
-
-    seen_constants = set()
-    seen_quantities = set()
-
-    for dbname in infiles:
-        pb.progress()
-
-        from logpyle import LogManager
-        logmgr = LogManager(dbname, "r")
-
-        # transfer warnings
-        transfer_data_table(db_conn, "warnings", logmgr.get_warnings())
-
-        # transfer constants
-        for key, val in logmgr.constants.items():
-            if key not in seen_constants:
-                db_conn.execute("insert into constants values (?,?)",
-                        (key, memoryview(dumps(val))))
-                seen_constants.add(key)
-
-        for qname, qdata in logmgr.quantity_data.items():
-            db_conn.execute("""insert into quantities values (?,?,?,?)""", (
-                  qname, qdata.unit, qdata.description,
-                  memoryview(dumps(qdata.default_aggregator))))
-
-            if qname not in seen_quantities:
-                db_conn.execute("""create table %s
-                  (step integer, rank integer, value real)""" % qname)
-                seen_quantities.add(qname)
-
-            transfer_data_table(db_conn, qname, logmgr.get_table(qname))
-
-        logmgr.close()
-
-    pb.finished()
-
-    db_conn.commit()
-    db_conn.close()
-
-
-def _normalize_types(x):
+def _normalize_types(x: Any) -> Any:
     # get rid of numpy types
     if isinstance(x, int):
         return int(x)
     if isinstance(x, float):
         return float(x)
     return x
 
 
-def gather_multi_file(outfile, infiles, fmap, qmap, fg, features,
-        dbname_to_run_id):
+def gather_multi_file(outfile: str, infiles: List[str], fmap: Dict[str, str],
+                      qmap: Dict[str, str], fg: FeatureGatherer,
+                      features: Dict[str, Any],
+                      dbname_to_run_id: Dict[str, int]) -> None:
     from pytools import ProgressBar
-    pb = ProgressBar("Importing...", len(infiles))
+    pb = ProgressBar("Importing...", len(infiles))  # type: ignore[no-untyped-call]
 
     feature_col_name_map = {}
     for fname in features:
         tgt_name = fmap.get(fname, fname)
 
         if tgt_name.lower() in sqlite_keywords:
             feature_col_name_map[fname] = tgt_name+"_"
@@ -279,63 +232,85 @@
             "dirname text",
             "filename text",
             ] + ["{} {}".format(feature_col_name_map[fname], ftype)
                     for fname, ftype in features.items()]
     db_conn.execute("create table runs (%s)" % ",".join(run_columns))
     db_conn.execute("create index runs_id on runs (id)")
 
+    # Caveat: the next three tables need to match the tables in _set_up_schema,
+    # plus the 'id'/'run_id' columns.
     db_conn.execute("""create table quantities (
             id integer primary key,
             name text,
             unit text,
             description text,
             rank_aggregator text
             )""")
 
-    db_conn.execute("""create table warnings (
-            run_id integer, step integer, rank integer, message text,
-            category text, filename text, lineno integer
-            )""")
+    db_conn.execute("""
+      create table warnings (
+        run_id integer,
+        rank integer,
+        step integer,
+        unixtime integer,
+        message text,
+        category text,
+        filename text,
+        lineno integer
+        )""")
+
+    db_conn.execute("""
+      create table logging (
+        run_id integer,
+        rank integer,
+        step integer,
+        unixtime integer,
+        level text,
+        message text,
+        filename text,
+        lineno integer
+        )""")
 
     created_tables = set()
 
-    from os.path import dirname, basename
+    from os.path import basename, dirname
 
     written_run_ids = set()
 
     for dbname in infiles:
-        pb.progress()
+        pb.progress()  # type: ignore[no-untyped-call]
 
         run_id = dbname_to_run_id[dbname]
 
-        from logpyle import LogManager
         logmgr = LogManager(dbname, "r")
 
         if run_id not in written_run_ids:
             dbfeatures = fg.get_db_features(dbname, logmgr)
             qry = "insert into runs ({}) values ({})".format(
                 ",".join(["id", "dirname", "filename"]
                     + [feature_col_name_map[f[0]] for f in dbfeatures]),
                 ",".join("?" * (len(dbfeatures)+3)))
             db_conn.execute(qry,
                     [run_id, dirname(dbname), basename(dbname)]
                     + [_normalize_types(f[2]) for f in dbfeatures])
 
             written_run_ids.add(run_id)
 
-        def transfer_data_table_multi(db_conn, tbl_name, data_table):
+        def transfer_data_table_multi(db_conn: Connection, tbl_name: str,
+                                      data_table: DataTable) -> None:
             my_data = [(run_id,)+d for d in data_table.data]
 
             db_conn.executemany(f"insert into {tbl_name} (%s) values (%s)" %
                 ("run_id,"
                     + ", ".join(data_table.column_names),
                     ", ".join("?" * (len(data_table.column_names)+1))),
                 my_data)
 
         transfer_data_table_multi(db_conn, "warnings", logmgr.get_warnings())
+        transfer_data_table_multi(db_conn, "logging", logmgr.get_logging())
 
         for qname, qdat in logmgr.quantity_data.items():
             tgt_qname = qmap.get(qname, qname)
 
             if tgt_qname not in created_tables:
                 created_tables.add(tgt_qname)
                 db_conn.execute("create table %s ("
@@ -344,42 +319,40 @@
 
                 db_conn.execute(
                         "create index {}_main on {} (run_id,step,rank)"
                         .format(tgt_qname, tgt_qname))
 
                 agg = qdat.default_aggregator
                 try:
-                    agg = agg.__name__
+                    agg = agg.__name__  # type: ignore[union-attr, assignment]
                 except AttributeError:
                     if agg is not None:
-                        agg = str(agg)
+                        agg = str(agg)  # type: ignore[assignment]
 
                 db_conn.execute("insert into quantities "
                         "(name,unit,description,rank_aggregator)"
                         "values (?,?,?,?)",
                         (tgt_qname, qdat.unit, qdat.description, agg))
 
             cursor = logmgr.db_conn.execute(
                     f"select {run_id},step,rank,value from {qname}")
             db_conn.executemany("insert into %s values (?,?,?,?)" % tgt_qname,
                     cursor)
         logmgr.close()
-    pb.finished()
+    pb.finished()  # type: ignore[no-untyped-call]
 
     db_conn.commit()
     db_conn.close()
 
 
-def main():
+def main() -> None:
     import sys
     from optparse import OptionParser
 
     parser = OptionParser(usage="%prog OUTDB DBFILES ...")
-    parser.add_option("-1", "--single", action="store_true",
-            help="Gather single-run instead of multi-run file")
     parser.add_option("-s", "--show-features", action="store_true",
             help="Only print the features found and quit")
     parser.add_option("-d", "--dir-features", action="store_true",
             help="Extract features from directory names")
     parser.add_option("-f", "--file-features", default=None,
             metavar="FILENAME",
             help="Read additional features from file, with lines like: "
@@ -413,20 +386,12 @@
     qmap = make_name_map(options.quantity_map)
 
     if options.show_features:
         for feat_name, feat_type in features.items():
             print(fmap.get(feat_name, feat_name), feat_type)
         sys.exit(0)
 
-    if options.single:
-        if len(set(dbname_to_run_id.values())) > 1:
-            raise ValueError(
-                    "data seems to come from more than one run--"
-                    "can't write single-run file")
-        gather_single_file(outfile, infiles)
-    else:
-        gather_multi_file(outfile, infiles, fmap, qmap, fg, features,
-                dbname_to_run_id)
+    gather_multi_file(outfile, infiles, fmap, qmap, fg, features, dbname_to_run_id)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `logpyle-2023.1/logpyle/__init__.py` & `logpyle-2023.2/logpyle/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,28 @@
 .. autoclass:: TimestepCounter
 .. autoclass:: StepToStepDuration
 .. autoclass:: TimestepDuration
 .. autoclass:: InitTime
 .. autoclass:: CPUTime
 .. autoclass:: ETA
 .. autoclass:: MemoryHwm
+.. autoclass:: GCStats
 .. autofunction:: add_general_quantities
 
 Built-in Log Simulation-Related Quantities
 ------------------------------------------
 .. autoclass:: SimulationTime
 .. autoclass:: Timestep
 .. autofunction:: set_dt
 .. autofunction:: add_simulation_quantities
+
+
+Internal stuff that is only here because the documentation tool wants it
+------------------------------------------------------------------------
+.. autoclass:: _SubTimer
 """
 
 __copyright__ = "Copyright (C) 2009-2013 Andreas Kloeckner"
 
 __license__ = """
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
@@ -55,46 +61,37 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 """
 
 
 import logpyle.version
+
 __version__ = logpyle.version.VERSION_TEXT
 
 
 import logging
+
 logger = logging.getLogger(__name__)
 
-from typing import (List, Callable, Union, Tuple, Optional, Dict, Any,
-                    TYPE_CHECKING, Iterable)
+from dataclasses import dataclass
+from sqlite3 import Connection
+from time import monotonic as time_monotonic
+from typing import (TYPE_CHECKING, Any, Callable, Dict, Generator, Iterable,
+                    List, Optional, Sequence, TextIO, Tuple, Type, Union, cast)
+
+from pymbolic.compiler import CompiledExpression  # type: ignore[import]
+from pymbolic.mapper.dependency import DependencyMapper  # type: ignore[import]
+from pymbolic.primitives import Expression  # type: ignore[import]
 from pytools.datatable import DataTable
 
 if TYPE_CHECKING:
     import mpi4py
 
 
-# {{{ timing function
-
-def time() -> float:
-    """Return elapsed CPU time, as a float, in seconds."""
-    import os
-    time_opt = os.environ.get("PYTOOLS_LOG_TIME") or "wall"
-    if time_opt == "wall":
-        from time import time
-        return time()
-    elif time_opt == "rusage":
-        from resource import getrusage, RUSAGE_SELF
-        return getrusage(RUSAGE_SELF).ru_utime
-    else:
-        raise RuntimeError("invalid timing method '%s'" % time_opt)
-
-# }}}
-
-
 # {{{ abstract logging interface
 
 class LogQuantity:
     """A source of a loggable scalar that is gathered at the start of each time step.
 
     Quantity values are gathered in :meth:`LogManager.tick_before`.
 
@@ -228,86 +225,87 @@
     .. automethod:: __call__
     .. automethod:: prepare_for_tick
     """
     pass
 
 
 class DtConsumer:
-    def __init__(self, dt) -> None:
-        self.dt = dt
+    def __init__(self) -> None:
+        self.dt: Optional[float] = None
 
-    def set_dt(self, dt) -> None:
+    def set_dt(self, dt: Optional[float]) -> None:
         self.dt = dt
 
 
 class TimeTracker(DtConsumer):
-    def __init__(self, dt: Optional[float], start: float = 0) -> None:
-        DtConsumer.__init__(self, dt)
+    def __init__(self, start: float = 0) -> None:
+        DtConsumer.__init__(self)
         self.t = start
 
     def tick(self) -> None:
-        self.t += self.dt
+        self.t += cast(float, self.dt)
 
 
 class SimulationLogQuantity(PostLogQuantity, DtConsumer):
     """A source of loggable scalars that needs to know the simulation timestep."""
 
-    def __init__(self, dt: Optional[float], name: str, unit: Optional[str] = None,
+    def __init__(self, name: str, unit: Optional[str] = None,
                  description: Optional[str] = None) -> None:
         PostLogQuantity.__init__(self, name, unit, description)
-        DtConsumer.__init__(self, dt)
+        DtConsumer.__init__(self)
 
 
 class PushLogQuantity(LogQuantity):
     def __init__(self, name: str, unit: Optional[str] = None,
                  description: Optional[str] = None) -> None:
         LogQuantity.__init__(self, name, unit, description)
-        self.value = None
+        self.value: Optional[float] = None
 
-    def push_value(self, value) -> None:
+    def push_value(self, value: float) -> None:
         if self.value is not None:
             raise RuntimeError("can't push two values per cycle")
         self.value = value
 
     def __call__(self) -> Optional[float]:
         v = self.value
         self.value = None
         return v
 
 
 class CallableLogQuantityAdapter(LogQuantity):
     """Adapt a 0-ary callable as a :class:`LogQuantity`."""
-    def __init__(self, callable: Callable, name: str, unit: Optional[str] = None,
-                 description: Optional[str] = None) -> None:
+    def __init__(self, callable: Callable[[], float], name: str,
+                 unit: Optional[str] = None, description: Optional[str] = None) \
+                    -> None:
         self.callable = callable
         LogQuantity.__init__(self, name, unit, description)
 
     def __call__(self) -> float:
         return self.callable()
 
 # }}}
 
 
 # {{{ manager functionality
 
+@dataclass(frozen=True)
 class _GatherDescriptor:
-    def __init__(self, quantity: LogQuantity, interval: int) -> None:
-        self.quantity = quantity
-        self.interval = interval
+    quantity: LogQuantity
+    interval: int
 
 
+@dataclass(frozen=True)
 class _QuantityData:
-    def __init__(self, unit: str, description: str,
-                 default_aggregator: Callable) -> None:
-        self.unit = unit
-        self.description = description
-        self.default_aggregator = default_aggregator
+    unit: Optional[str]
+    description: Optional[str]
+    default_aggregator: Optional[Callable[..., Any]]
 
 
-def _join_by_first_of_tuple(list_of_iterables):
+def _join_by_first_of_tuple(list_of_iterables: List[Iterable[Tuple[int, Any]]]) \
+        -> Generator[Tuple[int, List[Any]], None, None]:
     loi = [i.__iter__() for i in list_of_iterables]
     if not loi:
         return
     key_vals = [next(iter) for iter in loi]
     keys = [kv[0] for kv in key_vals]
     values = [kv[1] for kv in key_vals]
     target_key = max(keys)
@@ -335,78 +333,94 @@
 
         if min(keys) == target_key:
             yield target_key, values[:]
             force_advance = True
 
 
 def _get_unique_id() -> str:
-    try:
-        from uuid import uuid1
-    except ImportError:
-        try:
-            import hashlib
-            checksum = hashlib.md5()
-        except ImportError:
-            # for Python << 2.5
-            import md5  # type: ignore
-            checksum = md5.new()
-
-        from random import Random
-        rng = Random()
-        rng.seed()
-        for _ in range(20):
-            checksum.update(str(rng.randrange(1 << 30)).encode("utf-32"))
-        return checksum.hexdigest()
-    else:
-        return uuid1().hex
+    from uuid import uuid1
+    return uuid1().hex
 
 
-def _get_unique_suffix():
+def _get_unique_suffix() -> str:
     from datetime import datetime
     return "-" + datetime.utcnow().strftime("%Y%m%d-%H%M%S")
 
 
-def _set_up_schema(db_conn):
+def _set_up_schema(db_conn: Connection) -> int:
     # initialize new database
     db_conn.execute("""
       create table quantities (
         name text,
         unit text,
         description text,
         default_aggregator blob)""")
     db_conn.execute("""
       create table constants (
         name text,
         value blob)""")
+
+    # schema_version < 2 is missing the 'rank' field.
+    # schema_version < 3 is missing the 'unixtime' field.
     db_conn.execute("""
       create table warnings (
         rank integer,
         step integer,
+        unixtime integer,
         message text,
         category text,
         filename text,
         lineno integer
         )""")
 
-    schema_version = 2
+    # schema_version < 3 does not have the logging table
+    db_conn.execute("""
+      create table logging (
+        rank integer,
+        step integer,
+        unixtime integer,
+        level text,
+        message text,
+        filename text,
+        lineno integer
+        )""")
+
+    schema_version = 3
     return schema_version
 
 
-from pytools import Record
+@dataclass
+class _DependencyData:
+    name: str
+    qdat: _QuantityData
+    agg_func: Callable[..., Any]
+    varname: str
+    expr: Expression
+    nonlocal_agg: bool
+    table: Optional[DataTable] = None
+
+
+@dataclass
+class _WatchInfo:
+    parsed: Expression
+    expr: Expression
+    dep_data: List[_DependencyData]
+    compiled: CompiledExpression
+    unit: Optional[str]
+    format: str
 
 
 class LogManager:
     """A distributed-memory-capable diagnostic time-series logging facility.
     It is meant to log data from a computation, with certain log quantities
     available before a cycle, and certain other ones afterwards. A timeline of
     invocations looks as follows::
 
         tick_before()
         compute...
-        tick()
         tick_after()
 
         tick_before()
         compute...
         tick_after()
 
         ...
@@ -432,51 +446,54 @@
     .. automethod:: save
     .. automethod:: close
 
     .. rubric:: Data retrieval
 
     .. automethod:: get_table
     .. automethod:: get_warnings
+    .. automethod:: get_logging
     .. automethod:: get_expr_dataset
     .. automethod:: get_joint_dataset
 
     .. rubric:: Configuration
 
     .. automethod:: capture_warnings
+    .. automethod:: capture_logging
     .. automethod:: add_watches
     .. automethod:: set_watch_interval
     .. automethod:: set_constant
     .. automethod:: add_quantity
 
     .. rubric:: Time Loop
 
     .. automethod:: tick_before
     .. automethod:: tick_after
     """
 
     def __init__(self, filename: Optional[str] = None, mode: str = "r",
                  mpi_comm: Optional["mpi4py.MPI.Comm"] = None,
-                 capture_warnings: bool = True, commit_interval: float = 90,
-                 watch_interval: float = 1.0) -> None:
+                 capture_warnings: bool = True, commit_interval: int = 90,
+                 watch_interval: float = 1.0,
+                 capture_logging: bool = True) -> None:
         """Initialize this log manager instance.
 
-        :param filename: If given, the filename to which this log is bound.
+        :arg filename: If given, the filename to which this log is bound.
           If this database exists, the current state is loaded from it.
-        :param mode: One of "w", "r" for write, read. "w" assumes that the
+        :arg mode: One of "w", "r" for write, read. "w" assumes that the
           database is initially empty. May also be "wu" to indicate that
           a unique filename should be chosen automatically. May also be "wo"
           to indicate that the file should be overwritten.
         :arg mpi_comm: An optional :class:`mpi4py.MPI.Comm` object.
           If given, logs are periodically synchronized to the head node,
           which then writes them out to disk.
-        :param capture_warnings: Tap the Python warnings facility and save warnings
+        :arg capture_warnings: Tap the Python warnings facility and save warnings
           to the log file.
-        :param commit_interval: actually perform a commit only every N times a commit
+        :arg commit_interval: actually perform a commit only every N times a commit
           is requested.
-        :param watch_interval: print watches every N seconds.
+        :arg watch_interval: print watches every N seconds.
         """
 
         assert isinstance(mode, str), "mode must be a string"
         assert mode in ["w", "r", "wu", "wo"], "invalid mode"
 
         self.quantity_data: Dict[str, _QuantityData] = {}
         self.last_values: Dict[str, Optional[float]] = {}
@@ -485,33 +502,33 @@
         self.tick_count = 0
 
         self.commit_interval = commit_interval
         self.commit_countdown = commit_interval
 
         self.constants: Dict[str, object] = {}
 
-        self.last_save_time = time()
+        self.last_save_time = time_monotonic()
 
         # self-timing
-        self.start_time = time()
+        self.start_time = time_monotonic()
         self.t_log: float = 0
 
         # parallel support
         self.head_rank = 0
         self.mpi_comm = mpi_comm
         self.is_parallel = mpi_comm is not None
 
         if mpi_comm is None:
             self.rank = 0
         else:
             self.rank = mpi_comm.rank
             self.head_rank = 0
 
         # watch stuff
-        self.watches: List[Record] = []
+        self.watches: List[_WatchInfo] = []
         self.have_nonlocal_watches = False
 
         # Interval between printing watches, in seconds
         self.set_watch_interval(watch_interval)
 
         # database binding
         import sqlite3 as sqlite
@@ -587,61 +604,112 @@
                     # try again, someone might have created a file with the same name
                     continue
 
                 self._load()
 
             break
 
-        self.old_showwarning: Optional[Callable] = None
+        self.old_showwarning: Optional[Callable[..., Any]] = None
         if capture_warnings:
             self.capture_warnings(True)
 
+        self.logging_handler: Optional[logging.Handler] = None
+        if capture_logging:
+            self.capture_logging(True)
+
     def capture_warnings(self, enable: bool = True) -> None:
-        def _showwarning(message, category, filename, lineno, file=None, line=None):
-            try:
-                self.old_showwarning(message, category, filename, lineno, file, line)
-            except TypeError:
-                # cater to Python 2.5 and earlier
-                self.old_showwarning(message, category, filename, lineno)
+        def _showwarning(message: Union[Warning, str], category: Type[Warning],
+                         filename: str, lineno: int, file: Optional[TextIO] = None,
+                         line: Optional[str] = None) -> None:
+            assert self.old_showwarning
+            self.old_showwarning(message, category, filename, lineno, file, line)
+
+            from time import time
 
             if self.schema_version >= 1 and self.mode[0] == "w":
                 if self.schema_version >= 2:
-                    self.db_conn.execute("insert into warnings values (?,?,?,?,?,?)",
-                            (self.rank, self.tick_count, str(message), str(category),
-                                filename, lineno))
+                    self.db_conn.execute(
+                            "insert into warnings values (?,?,?,?,?,?,?)",
+                            (self.rank, self.tick_count, time(), str(message),
+                             str(category), filename, lineno))
                 else:
                     self.db_conn.execute("insert into warnings values (?,?,?,?,?)",
                             (self.tick_count, str(message), str(category),
                                 filename, lineno))
 
         import warnings
         if enable:
             if self.old_showwarning is None:
-                pass
                 self.old_showwarning = warnings.showwarning
                 warnings.showwarning = _showwarning
             else:
                 raise RuntimeError("Warnings capture was enabled twice")
         else:
             if self.old_showwarning is None:
                 raise RuntimeError(
                         "Warnings capture was disabled, but never enabled")
 
             warnings.showwarning = self.old_showwarning
             self.old_showwarning = None
 
+    def capture_logging(self, enable: bool = True) -> None:
+        class LogpyleLogHandler(logging.Handler):
+            def __init__(self, mgr: LogManager) -> None:
+                logging.Handler.__init__(self)
+                self.mgr = mgr
+
+            def emit(self, record: logging.LogRecord) -> None:
+                from time import time
+                self.mgr.db_conn.execute(
+                    "insert into logging values (?,?,?,?,?,?,?)",
+                    (self.mgr.rank, self.mgr.tick_count, time(), record.
+                     levelname, record.getMessage(), record.pathname,
+                     record.lineno))
+
+        root_logger = logging.getLogger()
+
+        if enable:
+            if self.mode[0] == "w" and self.logging_handler is None:
+                self.logging_handler = LogpyleLogHandler(self)
+                root_logger.addHandler(self.logging_handler)
+            elif self.logging_handler:
+                from warnings import warn
+                warn("Logging capture already enabled")
+        else:
+            if self.logging_handler:
+                root_logger.removeHandler(self.logging_handler)
+            self.logging_handler = None
+
+    def get_logging(self) -> DataTable:
+        # Match the table set up by _set_up_schema
+        columns = ["rank", "step", "unixtime", "level", "message", "filename",
+                   "lineno"]
+
+        result = DataTable(columns)  # type: ignore[no-untyped-call]
+
+        if self.schema_version < 3:
+            from warnings import warn
+            warn("This database lacks a 'logging' table")
+            return result
+
+        for row in self.db_conn.execute(
+                "select %s from logging" % (", ".join(columns))):
+            result.insert_row(row)  # type: ignore[no-untyped-call]
+
+        return result
+
     def _load(self) -> None:
         if self.mpi_comm and self.mpi_comm.rank != self.head_rank:
             return
 
         from pickle import loads
         for name, value in self.db_conn.execute("select name, value from constants"):
             self.constants[name] = loads(value)
 
-        self.schema_version = self.constants.get("schema_version", 0)
+        self.schema_version = cast(int, self.constants.get("schema_version", 0))
 
         self.is_parallel = bool(self.constants["is_parallel"])
 
         for name, unit, description, def_agg in self.db_conn.execute(
                 "select name, unit, description, default_aggregator "
                 "from quantities"):
             self.quantity_data[name] = _QuantityData(
@@ -654,50 +722,51 @@
         self.save()
         self.db_conn.close()
 
     def get_table(self, q_name: str) -> DataTable:
         if q_name not in self.quantity_data:
             raise KeyError("invalid quantity name '%s'" % q_name)
 
-        result = DataTable(["step", "rank", "value"])
+        result = DataTable(
+            ["step", "rank", "value"])  # type: ignore[no-untyped-call]
 
         for row in self.db_conn.execute(
                 "select step, rank, value from %s" % q_name):
-            result.insert_row(row)
+            result.insert_row(row)  # type: ignore[no-untyped-call]
 
         return result
 
     def get_warnings(self) -> DataTable:
+        # Match the table set up by _set_up_schema
         columns = ["step", "message", "category", "filename", "lineno"]
         if self.schema_version >= 2:
             columns.insert(0, "rank")
 
-        result = DataTable(columns)
+            if self.schema_version >= 3:
+                columns.insert(2, "unixtime")
+
+        result = DataTable(columns)  # type: ignore[no-untyped-call]
 
         for row in self.db_conn.execute(
                 "select %s from warnings" % (", ".join(columns))):
-            result.insert_row(row)
+            result.insert_row(row)  # type: ignore[no-untyped-call]
 
         return result
 
     def add_watches(self, watches: List[Union[str, Tuple[str, str]]]) -> None:
         """Add quantities that are printed after every time step.
 
-        :param watches:
+        :arg watches:
             List of expressions to watch. Each element can either be
             a string of the expression to watch, or a tuple of the expression
             and a format string. In the format string, you can use the custom
             fields ``{display}``, ``{value}``, and ``{unit}`` to indicate where the
             watch expression, value, and unit should be printed. The default format
             string for each watch is ``{display}={value:g}{unit}``.
         """
-        from pytools import Record
-
-        class WatchInfo(Record):
-            pass
 
         default_format = "{display}={value:g}{unit} | "
 
         for watch in watches:
             if isinstance(watch, tuple):
                 expr, fmt = watch
             else:
@@ -712,35 +781,35 @@
             else:
                 unit = None
 
             from pytools import any
             self.have_nonlocal_watches = self.have_nonlocal_watches or \
                     any(dd.nonlocal_agg for dd in dep_data)
 
-            from pymbolic import compile  # type: ignore
+            from pymbolic import compile  # type: ignore[import]
             compiled = compile(parsed, [dd.varname for dd in dep_data])
 
-            watch_info = WatchInfo(parsed=parsed, expr=expr, dep_data=dep_data,
-                    compiled=compiled, unit=unit, format=fmt)
+            watch_info = _WatchInfo(parsed=parsed, expr=expr, dep_data=dep_data,
+                                    compiled=compiled, unit=unit, format=fmt)
 
             self.watches.append(watch_info)
 
     def set_watch_interval(self, interval: float) -> None:
         """Set the interval (in seconds) between the time watches are printed.
 
-        :param interval: watch printing interval in seconds.
+        :arg interval: watch printing interval in seconds.
         """
         self.watch_interval = interval
         self.next_watch_tick = self.tick_count + 1
 
     def set_constant(self, name: str, value: Any) -> None:
         """Make a named, constant value available in the log.
 
-        :param name: the name of the constant.
-        :param value: the value of the constant.
+        :arg name: the name of the constant.
+        :arg value: the value of the constant.
         """
         existed = name in self.constants
         self.constants[name] = value
 
         from pickle import dumps
         value = bytes(dumps(value))
 
@@ -775,61 +844,46 @@
         try:
             self.db_conn.execute(f"update {name} set value = {float(value)} \
                 where rank = {self.rank} and step = {self.tick_count}")
         except Exception:
             print("while adding datapoint for '%s':" % name)
             raise
 
-    def _gather_for_descriptor(self, gd) -> None:
+    def _gather_for_descriptor(self, gd: _GatherDescriptor) -> None:
         if self.tick_count % gd.interval == 0:
             q_value = gd.quantity()
             if isinstance(gd.quantity, MultiLogQuantity):
                 for name, value in zip(gd.quantity.names, q_value):
                     self._insert_datapoint(name, value)
             else:
                 self._insert_datapoint(gd.quantity.name, q_value)
 
-    def tick(self) -> None:
-        """Record data points from each added :class:`LogQuantity`.
-
-        May also checkpoint data to disk, and/or synchronize data points
-        to the head rank.
-        """
-        from warnings import warn
-        warn("LogManager.tick() is deprecated. "
-                "Use LogManager.tick_{before,after}().",
-                DeprecationWarning)
-
-        self.tick_before()
-        self.tick_after()
-
     def tick_before(self) -> None:
         """Record data points from each added :class:`LogQuantity` that
         is not an instance of :class:`PostLogQuantity`. Also, invoke
         :meth:`PostLogQuantity.prepare_for_tick` on :class:`PostLogQuantity`
         instances.
         """
-        tick_start_time = time()
+        tick_start_time = time_monotonic()
 
         for gd in self.before_gather_descriptors:
             self._gather_for_descriptor(gd)
 
         for gd in self.after_gather_descriptors:
-            from typing import cast
             cast(PostLogQuantity, gd.quantity).prepare_for_tick()
 
-        self.t_log = time() - tick_start_time
+        self.t_log = time_monotonic() - tick_start_time
 
     def tick_after(self) -> None:
         """Record data points from each added :class:`LogQuantity` that
         is an instance of :class:`PostLogQuantity`.
 
         May also checkpoint data to disk.
         """
-        tick_start_time = time()
+        tick_start_time = time_monotonic()
 
         for gd_lst in [self.before_gather_descriptors,
                 self.after_gather_descriptors]:
             for gd in gd_lst:
                 gd.quantity.tick()
 
         for gd in self.after_gather_descriptors:
@@ -843,15 +897,15 @@
         if tick_start_time > self.last_save_time + save_interval:
             self.save()
 
         # print watches
         if self.tick_count+1 >= self.next_watch_tick:
             self._watch_tick()
 
-        self.t_log += time() - tick_start_time
+        self.t_log += time_monotonic() - tick_start_time
 
         # Adjust log update time(s), t_log
         for gd in self.after_gather_descriptors:
             if isinstance(gd.quantity, LogUpdateDuration):
                 self._update_t_log(gd.quantity.name, gd.quantity())
 
         self.tick_count += 1
@@ -866,24 +920,25 @@
         from sqlite3 import OperationalError
         try:
             self.db_conn.commit()
         except OperationalError as e:
             from warnings import warn
             warn("encountered sqlite error during commit: %s" % e)
 
-        self.last_save_time = time()
+        self.last_save_time = time_monotonic()
 
     def add_quantity(self, quantity: LogQuantity, interval: int = 1) -> None:
         """Add a :class:`LogQuantity` to this manager.
 
-        :param quantity: add the specified :class:`LogQuantity`.
-        :param interval: interval (in time steps) when to gather this quantity.
+        :arg quantity: add the specified :class:`LogQuantity`.
+        :arg interval: interval (in time steps) when to gather this quantity.
         """
 
-        def add_internal(name, unit, description, def_agg):
+        def add_internal(name: str, unit: Optional[str], description: Optional[str],
+                         def_agg: Optional[Callable[..., Any]]) -> None:
             logger.debug("add log quantity '%s'" % name)
 
             if name in self.quantity_data:
                 raise RuntimeError("cannot add the same quantity '%s' twice" % name)
             self.quantity_data[name] = _QuantityData(unit, description, def_agg)
 
             from pickle import dumps
@@ -912,43 +967,48 @@
                     quantity.default_aggregators):
                 add_internal(name, unit, description, def_agg)
         else:
             add_internal(quantity.name,
                     quantity.unit, quantity.description,
                     quantity.default_aggregator)
 
-    def get_expr_dataset(self, expression, description=None, unit=None):
+    def get_expr_dataset(self, expression: Expression,
+                         description: Optional[str] = None,
+                         unit: Optional[str] = None) \
+                            -> Tuple[Union[str, Any], Union[str, Any, None],
+                                     List[Tuple[int, Any]]]:
         """Prepare a time-series dataset for a given expression.
 
         :arg expression: A :mod:`pymbolic` expression that may involve
           the time-series variables and the constants in this :class:`LogManager`.
           If there is data from multiple ranks for a quantity occurring in
           this expression, an aggregator may have to be specified.
         :returns: ``(description, unit, table)``, where *table*
           is a list of tuples ``(tick_nbr, value)``.
 
         Aggregators are specified as follows:
-        - ``qty.min``, ``qty.max``, ``qty.avg``, ``qty.sum``, ``qty.norm2``,
-        ``qty.median``
-        - ``qty[rank_nbr]``
-        - ``qty.loc``
+            - ``qty.min``, ``qty.max``, ``qty.avg``, ``qty.sum``, ``qty.norm2``,
+              ``qty.median``
+            - ``qty[rank_nbr]``
+            - ``qty.loc``
         """
 
         parsed = self._parse_expr(expression)
         parsed, dep_data = self._get_expr_dep_data(parsed)
 
         # aggregate table data
         for dd in dep_data:
             table = self.get_table(dd.name)
-            table.sort(["step"])
-            dd.table = table.aggregated(["step"], "value", dd.agg_func).data
+            table.sort(["step"])  # type: ignore[no-untyped-call]
+            dd.table = table.aggregated(["step"],  # type: ignore
+                                        "value", dd.agg_func).data
 
         # evaluate unit and description, if necessary
         if unit is None:
-            from pymbolic import substitute, parse
+            from pymbolic import parse, substitute
 
             unit_dict = {dd.varname: dd.qdat.unit for dd in dep_data}
             from pytools import all
             if all(v is not None for v in unit_dict.values()):
                 unit_dict = {k: parse(v) for k, v in unit_dict.items()}
                 unit = substitute(parsed, unit_dict)
             else:
@@ -959,23 +1019,24 @@
 
         # compile and evaluate
         from pymbolic import compile
         compiled = compile(parsed, [dd.varname for dd in dep_data])
 
         data = []
 
-        for key, values in _join_by_first_of_tuple(dd.table for dd in dep_data):
+        for key, values in _join_by_first_of_tuple(
+                [dd.table for dd in dep_data if dd.table]):
             try:
                 data.append((key, compiled(*values)))
             except ZeroDivisionError:
                 pass
 
         return (description, unit, data)
 
-    def get_joint_dataset(self, expressions):
+    def get_joint_dataset(self, expressions: Sequence[Expression]) -> List[Any]:
         """Return a joint data set for a list of expressions.
 
         :arg expressions: a list of either strings representing
           expressions directly, or triples (descr, unit, expr).
           In the former case, the description and the unit are
           found automatically, if possible. In the latter case,
           they are used as specified.
@@ -1000,18 +1061,21 @@
 
         zipped_dubs = list(zip(*dubs))
         zipped_dubs[2] = list(
                 _join_by_first_of_tuple(zipped_dubs[2]))
 
         return zipped_dubs
 
-    def get_plot_data(self, expr_x, expr_y, min_step=None, max_step=None):
+    def get_plot_data(self, expr_x: Expression, expr_y: Expression,
+                      min_step: Optional[int] = None,
+                      max_step: Optional[int] = None) \
+                            -> Tuple[Tuple[Any, str, str], Tuple[Any, str, str]]:
         """Generate plot-ready data.
 
-        :return: ``(data_x, descr_x, unit_x), (data_y, descr_y, unit_y)``
+        :returns: ``(data_x, descr_x, unit_x), (data_y, descr_y, unit_y)``
         """
         (descr_x, descr_y), (unit_x, unit_y), data = \
                 self.get_joint_dataset([expr_x, expr_y])
         if min_step is not None:
             data = [(step, tup) for step, tup in data if min_step <= step]
         if max_step is not None:
             data = [(step, tup) for step, tup in data if step <= max_step]
@@ -1023,60 +1087,60 @@
         else:
             data_x = []
             data_y = []
 
         return (data_x, descr_x, unit_x), \
                (data_y, descr_y, unit_y)
 
-    def write_datafile(self, filename, expr_x, expr_y) -> None:
-        (data_x, label_x), (data_y, label_y) = self.get_plot_data(
+    def write_datafile(self, filename: str, expr_x: Expression,
+                       expr_y: Expression) -> None:
+        (data_x, label_x, _), (data_y, label_y, _) = self.get_plot_data(
                 expr_x, expr_y)
 
         outf = open(filename, "w")
         outf.write(f"# {label_x} vs. {label_y}")
         for dx, dy in zip(data_x, data_y):
             outf.write("{}\t{}\n".format(repr(dx), repr(dy)))
         outf.close()
 
-    def plot_matplotlib(self, expr_x, expr_y) -> None:
-        from matplotlib.pyplot import xlabel, ylabel, plot
+    def plot_matplotlib(self, expr_x: Expression, expr_y: Expression) -> None:
+        from matplotlib.pyplot import plot, xlabel, ylabel
 
         (data_x, descr_x, unit_x), (data_y, descr_y, unit_y) = \
                 self.get_plot_data(expr_x, expr_y)
 
         xlabel(f"{descr_x} [{unit_x}]")
         ylabel(f"{descr_y} [{unit_y}]")
         plot(data_x, data_y)
 
     # {{{ private functionality
 
-    def _parse_expr(self, expr):
+    def _parse_expr(self, expr: Expression) -> Any:
         from pymbolic import parse, substitute
         parsed = parse(expr)
 
         # substitute in global constants
         parsed = substitute(parsed, self.constants)
 
         return parsed
 
-    def _get_expr_dep_data(self, parsed):
+    def _get_expr_dep_data(self, parsed: Expression) \
+            -> Tuple[Expression, List[_DependencyData]]:
         class Nth:
-            def __init__(self, n):
+            def __init__(self, n: int) -> None:
                 self.n = n
 
-            def __call__(self, lst):
+            def __call__(self, lst: List[Any]) -> Any:
                 return lst[self.n]
 
-        from pymbolic.mapper.dependency import DependencyMapper  # type: ignore
-
         deps = DependencyMapper(include_calls=False)(parsed)
 
         # gather information on aggregation expressions
         dep_data = []
-        from pymbolic.primitives import Variable, Lookup, Subscript  # type: ignore
+        from pymbolic.primitives import Lookup, Subscript, Variable
         for dep_idx, dep in enumerate(deps):
             nonlocal_agg = True
 
             if isinstance(dep, Variable):
                 name = dep.name
 
                 if name == "math":
@@ -1120,32 +1184,32 @@
                 name = dep.aggregate.name
 
                 from pymbolic import evaluate
                 agg_func = Nth(evaluate(dep.index))
 
             qdat = self.quantity_data[name]
 
-            class DependencyData(Record):
-                pass
+            assert agg_func
 
-            this_dep_data = DependencyData(name=name, qdat=qdat, agg_func=agg_func,
+            this_dep_data = _DependencyData(name=name, qdat=qdat, agg_func=agg_func,
                     varname="logvar%d" % dep_idx, expr=dep,
                     nonlocal_agg=nonlocal_agg)
             dep_data.append(this_dep_data)
 
         # substitute in the "logvar" variable names
-        from pymbolic import var, substitute
+        from pymbolic import substitute, var
         parsed = substitute(parsed,
                 {dd.expr: var(dd.varname) for dd in dep_data})
 
         return parsed, dep_data
 
     def _calculate_next_watch_tick(self) -> None:
-        ticks_per_interval = (self.tick_count/max(1, time()-self.start_time)
-                         * self.watch_interval)
+        ticks_per_interval = (self.tick_count
+                              / max(1, time_monotonic()-self.start_time)
+                              * self.watch_interval)
         self.next_watch_tick = self.tick_count + int(max(1, ticks_per_interval))
 
     def _watch_tick(self) -> None:
         """Print the watches after a tick."""
         if not self.have_nonlocal_watches and self.rank != self.head_rank:
             return
 
@@ -1156,30 +1220,30 @@
             gathered_data = self.mpi_comm.gather(data_block, self.head_rank)
         else:
             gathered_data = [data_block]
 
         if self.rank == self.head_rank:
             assert gathered_data
 
-            values: Dict[str, list] = {}
+            values: Dict[str, List[Optional[float]]] = {}
             for data_block in gathered_data:
                 for name, value in data_block.items():
                     values.setdefault(name, []).append(value)
 
-            def compute_watch_str(watch):
+            def compute_watch_str(watch: _WatchInfo) -> str:
                 display = watch.expr
                 unit = watch.unit if watch.unit not in ["1", None] else ""
                 value = watch.compiled(
                         *[dd.agg_func(values[dd.name])
                             for dd in watch.dep_data])
                 try:
                     return f"{watch.format}".format(display=display, value=value,
                                                     unit=unit)
                 except ZeroDivisionError:
-                    return "%s:div0" % watch.display
+                    return f"{display}:div0"
             if self.watches:
                 print("".join(
                         compute_watch_str(watch) for watch in self.watches),
                       flush=True)
 
         self._calculate_next_watch_tick()
 
@@ -1191,31 +1255,31 @@
 
 # }}}
 
 
 # {{{ actual data loggers
 
 class _SubTimer:
-    def __init__(self, itimer) -> None:
+    def __init__(self, itimer: "IntervalTimer") -> None:
         self.itimer = itimer
-        self.elapsed = 0
+        self.elapsed = 0.0
 
-    def start(self):
-        self.start_time = time()
+    def start(self) -> "_SubTimer":
+        self.start_time = time_monotonic()
         return self
 
-    def stop(self):
-        self.elapsed += time() - self.start_time
+    def stop(self) -> "_SubTimer":
+        self.elapsed += time_monotonic() - self.start_time
         del self.start_time
         return self
 
     def __enter__(self) -> None:
         self.start()
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
         self.stop()
         self.submit()
 
     def submit(self) -> None:
         self.itimer.add_time(self.elapsed)
         self.elapsed = 0
 
@@ -1230,24 +1294,24 @@
     .. automethod:: add_time
     """
 
     def __init__(self, name: str, description: Optional[str] = None) -> None:
         LogQuantity.__init__(self, name, "s", description)
         self.elapsed: float = 0
 
-    def get_sub_timer(self):
+    def get_sub_timer(self) -> _SubTimer:
         return _SubTimer(self)
 
-    def start_sub_timer(self):
+    def start_sub_timer(self) -> _SubTimer:
         sub_timer = _SubTimer(self)
         sub_timer.start()
         return sub_timer
 
     def add_time(self, t: float) -> None:
-        self.start_time = time()
+        self.start_time = time_monotonic()
         self.elapsed += t
 
     def __call__(self) -> float:
         result = self.elapsed
         self.elapsed = 0
         return result
 
@@ -1278,27 +1342,29 @@
                  description: Optional[str] = None) -> None:
         PostLogQuantity.__init__(self, name, "1", description)
         self.events = 0
 
     def add(self, n: int = 1) -> None:
         self.events += n
 
-    def transfer(self, counter) -> None:
+    def transfer(self, counter: Any) -> None:
         self.events += counter.pop()
 
     def prepare_for_tick(self) -> None:
         self.events = 0
 
     def __call__(self) -> int:
         result = self.events
         return result
 
 
-def time_and_count_function(f, timer, counter=None, increment=1) -> Callable:
-    def inner_f(*args, **kwargs):
+def time_and_count_function(f: Callable[..., Any], timer: IntervalTimer,
+                            counter: Optional[EventCounter] = None,
+                            increment: int = 1) -> Callable[..., Any]:
+    def inner_f(*args: Any, **kwargs: Any) -> Any:
         if counter is not None:
             counter.add(increment)
         sub_timer = timer.start_sub_timer()
         try:
             return f(*args, **kwargs)
         finally:
             sub_timer.stop().submit()
@@ -1316,58 +1382,58 @@
     def __call__(self) -> int:
         result = self.steps
         self.steps += 1
         return result
 
 
 class StepToStepDuration(PostLogQuantity):
-    """Records the CPU time between invocations of
-    :meth:`LogManager.tick_before` and
-    :meth:`LogManager.tick_after`.
+    """Records the wall time between the starts of consecutive time steps, i.e.,
+    the wall time between :meth:`LogManager.tick_before` of step x and
+    :meth:`LogManager.tick_before` of step x+1. The value stored is the value for
+    step x+1.
 
     .. automethod:: __init__
     """
 
     def __init__(self, name: str = "t_2step") -> None:
         PostLogQuantity.__init__(self, name, "s", "Step-to-step duration")
         self.last_start_time: Optional[float] = None
         self.last2_start_time: Optional[float] = None
 
     def prepare_for_tick(self) -> None:
         self.last2_start_time = self.last_start_time
-        self.last_start_time = time()
+        self.last_start_time = time_monotonic()
 
     def __call__(self) -> Optional[float]:
         if self.last2_start_time is None or self.last_start_time is None:
             return None
         else:
             return self.last_start_time - self.last2_start_time
 
 
 class TimestepDuration(PostLogQuantity):
-    """Records the CPU time between the starts of time steps.
-    :meth:`LogManager.tick_before` and
-    :meth:`LogManager.tick_after`.
+    """Records the wall time between invocations of :meth:`LogManager.tick_before`
+    and :meth:`LogManager.tick_after`, i.e., the duration of the time step.
 
     .. automethod:: __init__
     """
 
     # We would like to run last, so that if log gathering takes any
     # significant time, we catch that, too. (CUDA sync-on-time-taking,
     # I'm looking at you.)
     sort_weight = 1000
 
     def __init__(self, name: str = "t_step") -> None:
         PostLogQuantity.__init__(self, name, "s", "Time step duration")
 
     def prepare_for_tick(self) -> None:
-        self.last_start = time()
+        self.last_start = time_monotonic()
 
     def __call__(self) -> float:
-        now = time()
+        now = time_monotonic()
         result = now - self.last_start
         del self.last_start
         return result
 
 
 class InitTime(LogQuantity):
     """Stores the time it took for the application to initialize.
@@ -1376,65 +1442,69 @@
 
     .. automethod:: __init__
     """
 
     def __init__(self, name: str = "t_init") -> None:
         LogQuantity.__init__(self, name, "s", "Init time")
 
-        import os
         try:
             import psutil
         except ModuleNotFoundError:
             from warnings import warn
             warn("Measuring the init time requires the 'psutil' module.")
             self.done = True
         else:
-            p = psutil.Process(os.getpid())
-            self.start_time = p.create_time()
+            self.create_time = psutil.Process().create_time()
             self.done = False
 
     def __call__(self) -> Optional[float]:
         if self.done:
             return None
 
         self.done = True
-        now = time()
-        return now - self.start_time
+        from time import time
+
+        # Can't use time_monotonic() here since that does *not* return
+        # the time since the UNIX epoch (like time() and
+        # psutil.Process.create_time() do), but from another (undefined)
+        # reference point.
+        return time() - self.create_time
 
 
 class CPUTime(LogQuantity):
-    """Records (monotonically increasing) CPU time.
+    """Records (monotonically increasing) wall time since the quantity was
+    initialized.
 
     .. automethod:: __init__
     """
     def __init__(self, name: str = "t_cpu") -> None:
         LogQuantity.__init__(self, name, "s", "Wall time")
 
-        self.start = time()
+        self.start = time_monotonic()
 
     def __call__(self) -> float:
-        return time()-self.start
+        return time_monotonic()-self.start
 
 
 class ETA(LogQuantity):
     """Records an estimate of how long the computation will still take.
 
     .. automethod:: __init__
     """
     def __init__(self, total_steps: int, name: str = "t_eta") -> None:
         LogQuantity.__init__(self, name, "s", "Estimated remaining duration")
 
         self.steps = 0
         self.total_steps = total_steps
-        self.start = time()
+        self.start = time_monotonic()
 
     def __call__(self) -> float:
         fraction_done = self.steps/self.total_steps
         self.steps += 1
-        time_spent = time()-self.start
+        time_spent = time_monotonic()-self.start
         if fraction_done > 1e-9:
             return time_spent/fraction_done-time_spent
         else:
             return 0
 
 
 def add_general_quantities(mgr: LogManager) -> None:
@@ -1448,57 +1518,53 @@
     mgr.add_quantity(InitTime())
     mgr.add_quantity(MemoryHwm())
 
 
 class SimulationTime(TimeTracker, LogQuantity):
     """Record (monotonically increasing) simulation time."""
 
-    def __init__(self, dt: Optional[float], name: str = "t_sim",
-                 start: float = 0) -> None:
+    def __init__(self, name: str = "t_sim", start: float = 0) -> None:
         LogQuantity.__init__(self, name, "s", "Simulation Time")
-        TimeTracker.__init__(self, dt, start)
+        TimeTracker.__init__(self, start)
 
     def __call__(self) -> float:
         return self.t
 
 
 class Timestep(SimulationLogQuantity):
     """Record the magnitude of the simulated time step."""
 
-    def __init__(self, dt: Optional[float], name: str = "dt",
-                 unit: str = "s") -> None:
-        SimulationLogQuantity.__init__(self, dt, name, unit, "Simulation Timestep")
+    def __init__(self, name: str = "dt", unit: str = "s") -> None:
+        SimulationLogQuantity.__init__(self, name, unit, "Simulation Timestep")
 
-    def __call__(self) -> float:
+    def __call__(self) -> Optional[float]:
         return self.dt
 
 
 def set_dt(mgr: LogManager, dt: float) -> None:
-    """Set the simulation timestep on :class:`LogManager` ``mgr`` to ``dt``."""
+    """Set the simulation timestep on :class:`LogManager` ``mgr`` to ``dt``.
+
+    :arg mgr: the :class:`LogManager` instance.
+    :arg dt: the simulation timestep.
+    """
 
     for gd_lst in [mgr.before_gather_descriptors,
             mgr.after_gather_descriptors]:
         for gd in gd_lst:
             if isinstance(gd.quantity, DtConsumer):
                 gd.quantity.set_dt(dt)
 
 
-def add_simulation_quantities(mgr: LogManager, dt: Optional[float] = None) -> None:
+def add_simulation_quantities(mgr: LogManager) -> None:
     """Add :class:`LogQuantity` objects relating to simulation time.
 
-    :param mgr: the :class:`LogManager` instance.
-    :param dt: (deprecated, use :meth:`set_dt` instead)
+    :arg mgr: the :class:`LogManager` instance.
     """
-    if dt is not None:
-        from warnings import warn
-        warn("Specifying dt ahead of time is a deprecated practice. "
-                "Use logpyle.set_dt() instead.")
-
-    mgr.add_quantity(SimulationTime(dt))
-    mgr.add_quantity(Timestep(dt))
+    mgr.add_quantity(SimulationTime())
+    mgr.add_quantity(Timestep())
 
 
 def add_run_info(mgr: LogManager) -> None:
     """Add generic run metadata, such as command line, host, and time."""
 
     try:
         import psutil
@@ -1528,10 +1594,71 @@
             raise ValueError("MemoryHwm is only supported on Linux/Mac.")
 
     def __call__(self) -> float:
         from resource import RUSAGE_SELF, getrusage
         res = getrusage(RUSAGE_SELF)
         return res.ru_maxrss / self.fac
 
+
+class GCStats(MultiPostLogQuantity):
+    """Record Garbage Collection statistics.
+
+    Information regarding the meaning of these values can be found at:
+        - https://docs.python.org/3/library/gc.html
+        - https://alex.dzyoba.com/blog/arc-vs-gc
+
+          ..  # noqa: E501
+        - https://stackoverflow.com/questions/64561488/pythons-gc-get-objects-from-get-count
+        - https://github.com/python/cpython/blob/main/Modules/gcmodule.c
+    """
+    def __init__(self) -> None:
+        names = [  # gc.isenabled():
+                  "gc_isenabled",
+                   # gc.get_count():
+                  "gc_count_gen0", "gc_count_gen1", "gc_count_gen2",
+                   # gc.get_stats():
+                  "gc_collections_gen0", "gc_collected_gen0",
+                  "gc_uncollectable_gen0",
+                  "gc_collections_gen1", "gc_collected_gen1",
+                  "gc_uncollectable_gen1",
+                  "gc_collections_gen2", "gc_collected_gen2",
+                  "gc_uncollectable_gen2",
+                 ]
+
+        units = ["bool",
+                 "1", "1", "1",
+                 "1", "1", "1", "1", "1", "1", "1", "1", "1"]
+
+        descriptions = ["Is automatic GC enabled?",
+                        "GC count gen0", "GC count gen1", "GC count gen2",
+                        "GC collections gen0", "GC objects collected gen0",
+                        "GC objects uncollectable gen0",
+                        "GC collections gen1", "GC objects collected gen1",
+                        "GC objects uncollectable gen1",
+                        "GC collections gen2", "GC objects collected gen2",
+                        "GC objects uncollectable gen2",
+                        ]
+
+        assert len(names) == len(units) == len(descriptions) == 13
+
+        super().__init__(names, units, descriptions)
+
+    def __call__(self) -> Iterable[Optional[float]]:
+        import gc
+
+        enabled = gc.isenabled()
+        counts = gc.get_count()
+        stats = gc.get_stats()
+
+        return [enabled,
+                counts[0], counts[1], counts[2],
+                stats[0]["collections"], stats[0]["collected"],
+                stats[0]["uncollectable"],
+                stats[1]["collections"], stats[1]["collected"],
+                stats[1]["uncollectable"],
+                stats[2]["collections"], stats[2]["collected"],
+                stats[2]["uncollectable"]
+                ]
+
 # }}}
 
 # vim: foldmethod=marker
```

### Comparing `logpyle-2023.1/logpyle/runalyzer.py` & `logpyle-2023.2/logpyle/runalyzer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 #! /usr/bin/env python
 
 import code
 
-
 try:
     import readline
     import rlcompleter  # noqa: F401
     HAVE_READLINE = True
 except ImportError:
     HAVE_READLINE = False
 
 
 import logging
+
 logger = logging.getLogger(__name__)
 
-from pytools import cartesian_product, Record
+from dataclasses import dataclass
+from itertools import product
+from sqlite3 import Connection, Cursor
+from typing import (Any, Callable, Dict, Generator, List, Optional, Sequence,
+                    Set, Tuple, Type, Union)
+
+from pytools import Table
 
 
-class PlotStyle(Record):
-    pass
+@dataclass(frozen=True)
+class PlotStyle:
+    dashes: Tuple[int, ...]
+    color: str
 
 
 PLOT_STYLES = [
         PlotStyle(dashes=dashes, color=color)
-        for dashes, color in cartesian_product(
+        for dashes, color in product(
             [(), (12, 2), (4, 2),  (2, 2), (2, 8)],
             ["blue", "green", "red", "magenta", "cyan"],
             )]
 
 
 class RunDB:
-    def __init__(self, db, interactive):
+    def __init__(self, db: Connection, interactive: bool) -> None:
         self.db = db
         self.interactive = interactive
-        self.rank_agg_tables = set()
+        self.rank_agg_tables: Set[Tuple[str, Callable[..., Any]]] = set()
 
-    def q(self, qry, *extra_args):
+    def q(self, qry: str, *extra_args: Any) -> Cursor:
         return self.db.execute(self.mangle_sql(qry), extra_args)
 
-    def mangle_sql(self, qry):
+    def mangle_sql(self, qry: str) -> str:
         return qry
 
-    def get_rank_agg_table(self, qty, rank_aggregator):
+    def get_rank_agg_table(self, qty: str,
+                           rank_aggregator: Callable[..., Any]) -> str:
         tbl_name = f"rankagg_{rank_aggregator}_{qty}"
 
         if (qty, rank_aggregator) in self.rank_agg_tables:
             return tbl_name
 
         logger.info("Building temporary rank aggregation table {tbl_name}.")
 
@@ -54,15 +63,16 @@
                 "from %s group by run_id,step" % (
                     tbl_name, rank_aggregator, qty))
         self.db.execute("create index %s_run_step on %s (run_id,step)"
                 % (tbl_name, tbl_name))
         self.rank_agg_tables.add((qty, rank_aggregator))
         return tbl_name
 
-    def scatter_cursor(self, cursor, labels=None, *args, **kwargs):
+    def scatter_cursor(self, cursor: Cursor, labels: Optional[List[str]] = None,
+                       *args: Any, **kwargs: Any) -> None:
         import matplotlib.pyplot as plt
 
         data_args = tuple(zip(*list(cursor)))
         plt.scatter(*(data_args + args), **kwargs)
 
         if isinstance(labels, list) and len(labels) == 2:
             plt.xlabel(labels[0])
@@ -70,16 +80,17 @@
         elif labels is not None:
             raise TypeError("The 'labels' parameter must be a list with two"
                             "elements.")
 
         if self.interactive:
             plt.show()
 
-    def plot_cursor(self, cursor, labels=None, *args, **kwargs):
-        from matplotlib.pyplot import plot, show, legend
+    def plot_cursor(self, cursor: Cursor, labels: Optional[List[str]] = None,
+                    *args: Any, **kwargs: Any) -> None:
+        from matplotlib.pyplot import legend, plot, show
 
         auto_style = kwargs.pop("auto_style", True)
 
         if len(cursor.description) == 2:
             if auto_style:
                 style = PLOT_STYLES[0]
                 kwargs["dashes"] = style.dashes
@@ -94,20 +105,21 @@
             elif labels is not None:
                 raise TypeError("The 'labels' parameter must be a list with two"
                                 " elements.")
 
         elif len(cursor.description) > 2:
             small_legend = kwargs.pop("small_legend", True)
 
-            def format_label(kv_pairs):
+            def format_label(kv_pairs: Sequence[Tuple[str, Any]]) -> str:
                 return " ".join(f"{column}:{value}"
                             for column, value in kv_pairs)
             format_label = kwargs.pop("format_label", format_label)
 
-            def do_plot(x, y, row_rest):
+            def do_plot(x: List[float], y: List[float],
+                        row_rest: Tuple[Any, ...]) -> None:
                 my_kwargs = kwargs.copy()
                 style = PLOT_STYLES[style_idx[0] % len(PLOT_STYLES)]
                 if auto_style:
                     my_kwargs.setdefault("dashes", style.dashes)
                     my_kwargs.setdefault("color", style.color)
 
                 my_kwargs.setdefault("label",
@@ -116,33 +128,35 @@
                             row_rest))))
 
                 plot(x, y, *args, hold=True, **my_kwargs)
                 style_idx[0] += 1
 
             style_idx = [0]
             for x, y, rest in split_cursor(cursor):
-                do_plot(x, y, rest)
+                do_plot(x, y, rest)  # type: ignore[arg-type]
 
             if small_legend:
                 from matplotlib.font_manager import FontProperties
                 legend(pad=0.04, prop=FontProperties(size=8), loc="best",
                         labelsep=0)
         else:
             raise ValueError("invalid number of columns")
 
         if self.interactive:
             show()
 
-    def print_cursor(self, cursor):
+    def print_cursor(self, cursor: Cursor) -> None:
         print(table_from_cursor(cursor))
 
 
-def split_cursor(cursor):
-    x = []
-    y = []
+def split_cursor(cursor: Cursor) -> Generator[
+        Tuple[List[Any], List[Any], Optional[Tuple[Any, ...]]], None, None]:
+
+    x: List[Any] = []
+    y: List[Any] = []
     last_rest = None
     for row in cursor:
         row_tuple = tuple(row)
         row_rest = row_tuple[2:]
 
         if last_rest is None:
             last_rest = row_rest
@@ -156,44 +170,44 @@
 
         x.append(row_tuple[0])
         y.append(row_tuple[1])
     if x:
         yield x, y, last_rest
 
 
-def table_from_cursor(cursor):
-    from pytools import Table
+def table_from_cursor(cursor: Cursor) -> Table:
     tbl = Table()
-    tbl.add_row([column[0] for column in cursor.description])
+    tbl.add_row(tuple([column[0] for column in cursor.description]))
     for row in cursor:
         tbl.add_row(row)
     return tbl
 
 
 class MagicRunDB(RunDB):
-    def mangle_sql(self, qry):
+    def mangle_sql(self, qry: str) -> str:
         up_qry = qry.upper()
         if "FROM" in up_qry and "$$" not in up_qry:
             return qry
 
         magic_columns = set()
+        import re
 
-        def replace_magic_column(match):
+        # should be: re.Match[Any]
+        def replace_magic_column(match: Any) -> str:
             qty_name = match.group(1)
             rank_aggregator = match.group(2)
 
             if rank_aggregator is not None:
                 rank_aggregator = rank_aggregator[1:]
                 magic_columns.add((qty_name, rank_aggregator))
                 return f"{rank_aggregator}_{qty_name}.value AS {qty_name}"
             else:
                 magic_columns.add((qty_name, None))
                 return "%s.value AS %s" % (qty_name, qty_name)
 
-        import re
         magic_column_re = re.compile(r"\$([a-zA-Z][A-Za-z0-9_]*)(\.[a-z]*)?")
         qry, _ = magic_column_re.subn(replace_magic_column, qry)
 
         other_clauses = [  # noqa: F841
                 "UNION",  "INTERSECT", "EXCEPT", "WHERE", "GROUP",
                 "HAVING", "ORDER", "LIMIT", ";"]
 
@@ -220,15 +234,15 @@
                 else:
                     addendum = ""
 
             from_clause += " inner join {} on ({}.run_id = runs.id{}) ".format(
                     full_tbl_src, full_tbl, addendum)
             last_tbl = full_tbl
 
-        def get_clause_indices(qry):
+        def get_clause_indices(qry: str) -> Dict[str, int]:
             other_clauses = ["UNION",  "INTERSECT", "EXCEPT", "WHERE", "GROUP",
                     "HAVING", "ORDER", "LIMIT", ";"]
 
             result = {}
             up_qry = qry.upper()
             for clause in other_clauses:
                 clause_match = re.search(r"\b%s\b" % clause, up_qry)
@@ -251,15 +265,16 @@
                         qry[:first_clause_idx]
                         + from_clause
                         + qry[first_clause_idx:])
 
         return qry
 
 
-def make_runalyzer_symbols(db):
+def make_runalyzer_symbols(db: RunDB) \
+        -> Dict[str, Union[RunDB, str, None, Callable[..., Any]]]:
     return {
             "__name__": "__console__",
             "__doc__": None,
             "db": db,
             "mangle_sql": db.mangle_sql,
             "q": db.q,
             "dbplot": db.plot_cursor,
@@ -267,15 +282,15 @@
             "dbprint": db.print_cursor,
             "split_cursor": split_cursor,
             "table_from_cursor": table_from_cursor,
             }
 
 
 class RunalyzerConsole(code.InteractiveConsole):
-    def __init__(self, db):
+    def __init__(self, db: RunDB) -> None:
         self.db = db
         code.InteractiveConsole.__init__(self,
                 make_runalyzer_symbols(db))
 
         try:
             import numpy  # noqa: F401
             self.runsource("from numpy import *")
@@ -287,53 +302,55 @@
             self.runsource("from matplotlib.pyplot import *")
         except ImportError:
             pass
         except RuntimeError:
             pass
 
         if HAVE_READLINE:
-            import os
             import atexit
+            import os
 
             histfile = os.path.join(os.environ["HOME"], ".runalyzerhist")
             if os.access(histfile, os.R_OK):
                 readline.read_history_file(histfile)
             atexit.register(readline.write_history_file, histfile)
             readline.parse_and_bind("tab: complete")
 
         self.last_push_result = False
 
-    def push(self, cmdline):
+    def push(self, cmdline: str) -> bool:
         if cmdline.startswith("."):
             try:
                 self.execute_magic(cmdline)
             except Exception:
                 import traceback
                 traceback.print_exc()
         else:
             self.last_push_result = code.InteractiveConsole.push(self, cmdline)
 
         return self.last_push_result
 
-    def execute_magic(self, cmdline):
+    def execute_magic(self, cmdline: str) -> None:
         cmd_end = cmdline.find(" ")
         if cmd_end == -1:
             cmd = cmdline[1:]
             args = ""
         else:
             cmd = cmdline[1:cmd_end]
             args = cmdline[cmd_end+1:]
 
         if cmd == "help":
             print("""
 Commands:
  .help        show this help message
  .q SQL       execute a (potentially mangled) query
- .runprops    show a list of run properties
+ .constants   show a list of (constant) run properties
  .quantities  show a list of time-dependent quantities
+ .warnings    show a list of warnings
+ .logging     show a list of logging messages
 
 Plotting:
  .plot SQL    plot results of (potentially mangled) query.
               result sets can be (x,y) or (x,y,descr1,descr2,...),
               in which case a new plot will be started for each
               tuple (descr1, descr2, ...)
  .scatter SQL make scatterplot results of (potentially mangled) query.
@@ -350,27 +367,31 @@
     db: the SQLite database
     mangle_sql(query_str): mangle the SQL query string query_str
     q(query_str): get db cursor for mangled query_str
     dbplot(cursor): plot result of cursor
     dbscatter(cursor): make scatterplot result of cursor
     dbprint(cursor): print result of cursor
     split_cursor(cursor): x,y,data gather that .plot uses internally
-    table_from_cursor(cursor)
+    table_from_cursor(cursor): Create a printable table from a cursor
 """)
         elif cmd == "q":
             self.db.print_cursor(self.db.q(args))
 
-        elif cmd == "runprops":
+        elif cmd == "runprops" or cmd == "constants":
             cursor = self.db.db.execute("select * from runs")
             columns = [column[0] for column in cursor.description]
             columns.sort()
             for col in columns:
                 print(col)
         elif cmd == "quantities":
             self.db.print_cursor(self.db.q("select * from quantities order by name"))
+        elif cmd == "warnings":
+            self.db.print_cursor(self.db.q("select * from warnings"))
+        elif cmd == "logging":
+            self.db.print_cursor(self.db.q("select * from logging"))
         elif cmd == "title":
             from pylab import title
             title(args)
         elif cmd == "plot":
             cursor = self.db.db.execute(self.db.mangle_sql(args))
             columnnames = [column[0] for column in cursor.description]
             self.db.plot_cursor(cursor, labels=columnnames)
@@ -384,75 +405,76 @@
 
 # {{{ custom aggregates
 
 from pytools import VarianceAggregator  # noqa: E402
 
 
 class Variance(VarianceAggregator):
-    def __init__(self):
-        VarianceAggregator.__init__(self, entire_pop=True)
+    def __init__(self) -> None:
+        VarianceAggregator.__init__(self,  # type: ignore[no-untyped-call]
+                                    entire_pop=True)
 
 
 class StdDeviation(Variance):
-    def finalize(self):
-        result = Variance.finalize(self)
+    def finalize(self) -> Optional[float]:
+        result = Variance.finalize(self)  # type: ignore[no-untyped-call]
 
         if result is None:
             return None
         else:
             from math import sqrt
             return sqrt(result)
 
 
 class Norm1:
-    def __init__(self):
-        self.abs_sum = 0
+    def __init__(self) -> None:
+        self.abs_sum = 0.0
 
-    def step(self, value):
+    def step(self, value: float) -> None:
         self.abs_sum += abs(value)
 
-    def finalize(self):
+    def finalize(self) -> float:
         return self.abs_sum
 
 
 class Norm2:
-    def __init__(self):
-        self.square_sum = 0
+    def __init__(self) -> None:
+        self.square_sum = 0.0
 
-    def step(self, value):
+    def step(self, value: float) -> None:
         self.square_sum += value**2
 
-    def finalize(self):
+    def finalize(self) -> float:
         from math import sqrt
         return sqrt(self.square_sum)
 
 
-def my_sprintf(format, arg):
+def my_sprintf(format: str, arg: str) -> str:
     return format % arg
 
 # }}}
 
 
 # {{{ main program
 
-def make_wrapped_db(filename, interactive, mangle):
+def make_wrapped_db(filename: str, interactive: bool, mangle: bool) -> RunDB:
     import sqlite3
     db = sqlite3.connect(filename)
-    db.create_aggregate("stddev", 1, StdDeviation)
+    db.create_aggregate("stddev", 1, StdDeviation)  # type: ignore[arg-type]
     db.create_aggregate("var", 1, Variance)
-    db.create_aggregate("norm1", 1, Norm1)
-    db.create_aggregate("norm2", 1, Norm2)
+    db.create_aggregate("norm1", 1, Norm1)  # type: ignore[arg-type]
+    db.create_aggregate("norm2", 1, Norm2)  # type: ignore[arg-type]
 
     db.create_function("sprintf", 2, my_sprintf)
-    from math import sqrt, pow
+    from math import pow, sqrt
     db.create_function("sqrt", 1, sqrt)
     db.create_function("pow", 2, pow)
 
     if mangle:
-        db_wrap_class = MagicRunDB
+        db_wrap_class: Type[RunDB] = MagicRunDB
     else:
         db_wrap_class = RunDB
 
     return db_wrap_class(db, interactive=interactive)
 
 # }}}
```

### Comparing `logpyle-2023.1/logpyle.egg-info/PKG-INFO` & `logpyle-2023.2/logpyle.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: logpyle
-Version: 2023.1
+Version: 2023.2
 Summary: Time series logging for Python
 Home-page: https://github.com/illinois-ceesd/logpyle
 Author: Andreas Kloeckner
 Author-email: inform@tiker.net
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Python: ~=3.6
+Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # logpyle: Time Series Logging (not just) for Simulation
 
 [![CI](https://github.com/illinois-ceesd/logpyle/workflows/CI/badge.svg)](https://github.com/illinois-ceesd/logpyle/actions?query=workflow%3ACI+branch%3Amain)
 [![Documentation Status](https://readthedocs.org/projects/logpyle/badge/?version=latest)](https://logpyle.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `logpyle-2023.1/setup.py` & `logpyle-2023.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,25 +24,24 @@
           "Intended Audience :: Developers",
           "Intended Audience :: Other Audience",
           "Intended Audience :: Science/Research",
           "License :: OSI Approved :: MIT License",
           "Natural Language :: English",
           "Programming Language :: Python",
           "Programming Language :: Python :: 3",
-          "Programming Language :: Python :: 3.6",
           "Programming Language :: Python :: 3.7",
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Information Analysis",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Scientific/Engineering :: Visualization",
           "Topic :: Software Development :: Libraries",
           "Topic :: Utilities",
           ],
 
-      python_requires="~=3.6",
+      python_requires="~=3.7",
 
       install_requires=[
           "pytools>=2011.1",
           "pymbolic",
       ],
 
       package_data={"logpyle": ["py.typed"]},
```

