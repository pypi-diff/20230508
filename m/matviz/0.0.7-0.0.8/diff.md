# Comparing `tmp/matviz-0.0.7.tar.gz` & `tmp/matviz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matviz-0.0.7.tar", last modified: Wed Mar 24 17:15:07 2021, max compression
+gzip compressed data, was "matviz-0.0.8.tar", last modified: Mon May  8 21:41:59 2023, max compression
```

## Comparing `matviz-0.0.7.tar` & `matviz-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-24 17:15:07.571819 matviz-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-03-24 17:15:07.571819 matviz-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      592 2021-03-24 17:14:53.000000 matviz-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-24 17:15:07.571819 matviz-0.0.7/matviz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-24 17:14:53.000000 matviz-0.0.7/matviz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23277 2021-03-24 17:14:53.000000 matviz-0.0.7/matviz/etl.py
--rw-r--r--   0 runner    (1001) docker     (121)     3807 2021-03-24 17:14:53.000000 matviz-0.0.7/matviz/helpers_graphing.py
--rw-r--r--   0 runner    (1001) docker     (121)    27312 2021-03-24 17:14:53.000000 matviz-0.0.7/matviz/histogram_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    25420 2021-03-24 17:14:53.000000 matviz-0.0.7/matviz/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-24 17:15:07.571819 matviz-0.0.7/matviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-03-24 17:15:07.000000 matviz-0.0.7/matviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-03-24 17:15:07.000000 matviz-0.0.7/matviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-24 17:15:07.000000 matviz-0.0.7/matviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-03-24 17:15:07.000000 matviz-0.0.7/matviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-03-24 17:15:07.000000 matviz-0.0.7/matviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-03-24 17:15:07.571819 matviz-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2549 2021-03-24 17:14:53.000000 matviz-0.0.7/setup.py
+drwxr-xr-x   0 yoni       (501) staff       (20)        0 2023-05-08 21:41:59.772763 matviz-0.0.8/
+-rw-r--r--   0 yoni       (501) staff       (20)     1526 2020-09-24 14:16:13.000000 matviz-0.0.8/LICENSE
+-rw-r--r--   0 yoni       (501) staff       (20)     1804 2023-05-08 21:41:59.772866 matviz-0.0.8/PKG-INFO
+-rw-r--r--   0 yoni       (501) staff       (20)      592 2020-09-24 14:16:13.000000 matviz-0.0.8/README.md
+drwxr-xr-x   0 yoni       (501) staff       (20)        0 2023-05-08 21:41:59.771601 matviz-0.0.8/matviz/
+-rw-r--r--   0 yoni       (501) staff       (20)        0 2021-02-07 13:17:23.000000 matviz-0.0.8/matviz/__init__.py
+-rw-r--r--   0 yoni       (501) staff       (20)     1852 2021-09-27 23:57:09.000000 matviz-0.0.8/matviz/cbrt_scale.py
+-rw-r--r--   0 yoni       (501) staff       (20)     6048 2023-05-08 21:31:52.000000 matviz-0.0.8/matviz/circle_utils.py
+-rw-r--r--   0 yoni       (501) staff       (20)    25894 2023-05-08 21:31:52.000000 matviz-0.0.8/matviz/etl.py
+-rw-r--r--   0 yoni       (501) staff       (20)     4287 2023-05-08 21:31:52.000000 matviz-0.0.8/matviz/helpers_graphing.py
+-rw-r--r--   0 yoni       (501) staff       (20)    27557 2023-05-08 21:31:52.000000 matviz-0.0.8/matviz/histogram_utils.py
+-rw-r--r--   0 yoni       (501) staff       (20)      378 2021-09-27 23:55:34.000000 matviz-0.0.8/matviz/hnotest_3.py
+-rw-r--r--   0 yoni       (501) staff       (20)      378 2023-05-08 21:31:52.000000 matviz-0.0.8/matviz/test_3.py
+-rw-r--r--   0 yoni       (501) staff       (20)    31593 2023-05-08 21:31:52.000000 matviz-0.0.8/matviz/viz.py
+drwxr-xr-x   0 yoni       (501) staff       (20)        0 2023-05-08 21:41:59.772336 matviz-0.0.8/matviz.egg-info/
+-rw-r--r--   0 yoni       (501) staff       (20)     1804 2023-05-08 21:41:59.000000 matviz-0.0.8/matviz.egg-info/PKG-INFO
+-rw-r--r--   0 yoni       (501) staff       (20)      381 2023-05-08 21:41:59.000000 matviz-0.0.8/matviz.egg-info/SOURCES.txt
+-rw-r--r--   0 yoni       (501) staff       (20)        1 2023-05-08 21:41:59.000000 matviz-0.0.8/matviz.egg-info/dependency_links.txt
+-rw-r--r--   0 yoni       (501) staff       (20)       92 2023-05-08 21:41:59.000000 matviz-0.0.8/matviz.egg-info/requires.txt
+-rw-r--r--   0 yoni       (501) staff       (20)        7 2023-05-08 21:41:59.000000 matviz-0.0.8/matviz.egg-info/top_level.txt
+-rw-r--r--   0 yoni       (501) staff       (20)       79 2023-05-08 21:41:59.773157 matviz-0.0.8/setup.cfg
+-rw-r--r--   0 yoni       (501) staff       (20)     2594 2023-05-08 21:38:57.000000 matviz-0.0.8/setup.py
+drwxr-xr-x   0 yoni       (501) staff       (20)        0 2023-05-08 21:41:59.772463 matviz-0.0.8/test/
+-rw-r--r--   0 yoni       (501) staff       (20)      374 2021-09-28 00:08:22.000000 matviz-0.0.8/test/test_2.py
```

### Comparing `matviz-0.0.7/PKG-INFO` & `matviz-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: matviz
-Version: 0.0.7
+Version: 0.0.8
 Summary: matviz: matrix data visualization
 Home-page: https://github.com/JLansey/matviz
+Download-URL: https://github.com/JLansey/matviz
 Author: Jonathan Lansey
 Author-email: jonathan@lansey.net
 Maintainer: Jonathan Lansey
 Maintainer-email: jonathan@lansey.net
 License: BSD (3-clause)
-Download-URL: https://github.com/JLansey/matviz
-Description: MatViz is a library for making nice looking and useful graphics in Python. It is built on top of `matplotlib <https://matplotlib.org/>`_ and closely integrated with `numpy <https://numpy.org/>`_ and `pandas <https://pandas.pydata.org/>`_ data structures.
-        It also pulls from and is inspired by `seaborn <https://https://seaborn.pydata.org/>`_
-        Here is some of the functionality that matviz offers:
-        - A histogram function that compares multiple distributions with default settings to maximize utility
-        - A 2D histogram function with fun tricks like smoothing and plotting timeseries data
-        - Specialized support for using complex numbers in place of x and y (z = x + 1j * y)
-        - Taking any figure and making it look nicer than the matplotlib defaults
-        - Streamgraph implementation with lots of additional features, based on stackedplot
-        - Lots of plotting functions to import by default and make the coding environment similar to Matlab.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+License-File: LICENSE
+
+MatViz is a library for making nice looking and useful graphics in Python. It is built on top of `matplotlib <https://matplotlib.org/>`_ and closely integrated with `numpy <https://numpy.org/>`_ and `pandas <https://pandas.pydata.org/>`_ data structures.
+It also pulls from and is inspired by `seaborn <https://https://seaborn.pydata.org/>`_
+Here is some of the functionality that matviz offers:
+- A histogram function that compares multiple distributions with default settings to maximize utility
+- A 2D histogram function with fun tricks like smoothing and plotting timeseries data
+- Specialized support for using complex numbers in place of x and y (z = x + 1j * y)
+- Taking any figure and making it look nicer than the matplotlib defaults
+- Streamgraph implementation with lots of additional features, based on stackedplot
+- Lots of plotting functions to import by default and make the coding environment similar to Matlab.
```

### Comparing `matviz-0.0.7/README.md` & `matviz-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `matviz-0.0.7/matviz/etl.py` & `matviz-0.0.8/matviz/etl.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,54 +5,72 @@
 from pathlib import Path
 from numpy.lib.stride_tricks import as_strided as ast
 
 # regular pythong stuff
 # redundant form interactive computing
 import collections
 from collections import defaultdict
-from collections import Sequence
+from collections.abc import Sequence
 from itertools import chain, count
 from operator import itemgetter
+import numbers
 import glob
 import json
 # import simplejson as json
 import logging
 
 # datetime related things
 from dateutil.parser import parse as dateutil_parse
 import matplotlib.dates as md # for handledates
 import datetime
 from pytz import timezone
 import pickle
+from decimal import Decimal
 
 
 # regular anaconda stuff
 import numpy as np
 from scipy import signal
 import pandas as pd
 
 # for geometric median
 from scipy.spatial.distance import cdist, euclidean
 from scipy import interpolate
 
+from numpy.random import MT19937
+from numpy.random import RandomState, SeedSequence
+
+
 # useful stuffs:
 from numpy import diff
 
 
 data_dir = 'data'
 fig_dir = 'figs'
 
 eps = np.spacing(1)
 
 
 
 def time_delta_to_days(w):
     return w / np.timedelta64(1, 'D')
 
+def time_delta_to_seconds(w):
+    return w / np.timedelta64(1, 's')
+
+def timestamp_to_fraction(dates):
+    """
+    Convert a pandas timestamp to fractions
+    :param dates:
+    :return:
+    """
+    return (dates - dates.floor('D')) / pd.Timedelta(24, 'H')
 
+def microsoft_to_timestamp(ts):
+    return pd.Timestamp((ts - 116444736000000000)*100)
 
 def get_object_size(obj):
     """
     Get the number of megabytes bytes that the object is
     :param obj:
     :return:
     """
@@ -106,43 +124,52 @@
 def remove_tz(cur_datetime):
     if hasattr(cur_datetime,"__len__"):
         naive_datetime = [w.replace(tzinfo=None) for w in cur_datetime]
     else:
         naive_datetime = cur_datetime.replace(tzinfo=None)
     return naive_datetime
 
-def tz_to_utc(cur_datetime,local_tz='US/Eastern',native=True):
+def tz_to_utc(cur_datetime, local_tz='US/Eastern',native=True):
     local_datetime = timezone(local_tz).localize(cur_datetime)
     utc_datetime = local_datetime.astimezone(timezone('UTC'))
 
     if native:
         return utc_datetime.replace(tzinfo=None)
     else:
         return utc_datetime
 
-def utc_to_tz(cur_utc,local_tz='US/Eastern'):
+def utc_to_tz(cur_utc, local_tz='US/Eastern'):
     # this is a UTC time but without timezone information
     utc_datetime = timezone('UTC').localize(cur_utc)
     local_datetime = utc_datetime.astimezone(timezone(local_tz))
     naive_datetime = local_datetime.replace(tzinfo=None)
     return naive_datetime
 
-def to_tz(cur_tz,local_tz='US/Eastern'):
+def to_tz(cur_tz, local_tz='US/Eastern'):
     # if there is already time zone information associated here, then just go with it
     local_datetime = cur_tz.astimezone(timezone(local_tz))
     naive_datetime = local_datetime.replace(tzinfo=None)
     return naive_datetime
 
 def round_time(ts, round_by='H'):
-    ts_no_tz = remove_tz(ts)
-    return pd.Series(ts_no_tz).dt.round(round_by)
+    # check if time format includes time zone information
+    if hasattr(ts,"tzinfo"):
+        ts = remove_tz(ts)
+
+    return pd.Series(ts).dt.round(round_by)
 
 
 
 def average_times(time_1,time_2):
+    """
+    Average two times
+    :param time_1:
+    :param time_2:
+    :return:
+    """
     dummy_time = datetime.datetime(2000, 1, 1, 0, 0)
     return dummy_time + datetime.timedelta(seconds=((time_1-dummy_time).total_seconds()+(time_2-dummy_time).total_seconds())/2)
 
 
 
 
 def chunks(l, n):
@@ -622,15 +649,15 @@
 
 
 def interp_nans(t, y, t_i=None):
     """
     Interpolate t and y between any nans, and resample to consistent sampling rate
     :param t: time
     :param y: key variable
-    :return:
+    :return: t_i, y_i
     """
     I = np.logical_not(np.isnan(y))
     t = t[I]
     y = y[I]
     if t_i is None:
         ds = np.nanmedian(np.diff(t))
         t_i = np.arange(min(t), max(t), ds)
@@ -680,14 +707,15 @@
     diffs = abs(value - percentiles)
     ii = np.argmin(diffs)
     percentile = ii
 
     return percentile
 
 
+
 # kind of like a median in 2D
 # https://stackoverflow.com/a/30305181/3417198
 def geometric_median(X, eps=1e-5):
     y = np.mean(X, 0)
 
     while True:
         D = cdist(X, [y])
@@ -716,15 +744,15 @@
 
 
 
 
 # ***** MOVE THIS OVER TO ETL PLZ
 # https://stackoverflow.com/questions/32935232/python-apply-function-to-values-in-nested-dictionary
 def map_nested_dicts(ob, func):
-    if isinstance(ob, collections.Mapping):
+    if isinstance(ob, collections.abc.Mapping):
         return {k: map_nested_dicts(v, func) for k, v in ob.items()}
     else:
         return func(ob)
 
 
 #  these two functions are for dumping and loading arrays of complex numbers
 def complex_load(txt):
@@ -766,23 +794,43 @@
     data_dict = json.loads(json_str)
     #     convert any stored complex numbers back into native format
     data_dict = map_nested_dicts(data_dict, complex_load)
     return data_dict
 
 
 
-def dump_json(data_dict, file_path):
-    # pickle any complex numbers into strings
+def dump_json(data_dict, file_path, to_indent=None):
     data_dict = map_nested_dicts(data_dict, complex_dump)
     with open(file_path, 'w') as json_file:
-        json.dump(data_dict, json_file)
+        json.dump(data_dict, json_file, indent=to_indent)
     # txt = json.dumps(data_dict)
     # write_string(file_path, txt)
     return True
 
+def encode_floats(nums, decimals=3):
+    """
+    Convert numpy numbers to ones ready for dumping with simplejson
+    useful when you don't want your json exports to be bloated with too many
+    significant figures
+    :param nums: list of numbers
+    :param decimals: number of decimals you want to output
+    """
+    def convert_to_rounded_dec(num):
+        # convert to decimal
+        num_dec = Decimal(np.float64(num))
+        # create decimal number for quantizing
+        round_dec = Decimal("".join(['0.'] + ['0'] * (decimals - 1) + ['1']))
+        # actually round the number here
+        num_round = num_dec.quantize(round_dec, rounding='ROUND_HALF_UP')
+        return num_round
+    # apply the function to the list of numbers
+    func = (np.vectorize(convert_to_rounded_dec))
+    # remove the numpy data type by converting to a list
+    return func(nums).tolist()
+
 #Useful in Python 2, (or 3.4 or lower)
 # https://stackoverflow.com/questions/38987/how-to-merge-two-dictionaries-in-a-single-expression
 def merge_two_dicts(x, y):
     z = x.copy()   # start with x's keys and values
     z.update(y)    # modifies z with y's keys and values & returns None
     return z
 
@@ -814,19 +862,61 @@
 def isdigit(s):
     """
     check if the number is a digit, including if it has a decimal place in it
     Or is numeric
     :param s:
     :return:
     """
-    return s.replace('.','',1).replace('-', '').isdigit()
+    if isinstance(s, numbers.Number):
+        return True
+    else:
+        return s.replace('.','',1).replace('-', '').isdigit()
+
+
+def robust_floater(w):
+    """
+    If w could be numeric, then convert it to a float, otherwise leave it as is
+    """
+    if w is None:
+        return np.nan
+    else:
+         return float(w) if isdigit(w) else w
 
 
 def split_list(cur_list, func):
     list_true = []
     list_false = []
     for w in cur_list:
         if func(w):
             list_true.append(w)
         else:
             list_false.append(w)
-    return list_true, list_false
+    return list_true, list_false
+
+
+def rgb2hex(r,g,b):
+    return f"#{r:02x}{g:02x}{b:02x}"
+
+def first_non_zero_or_nan(x):
+    """
+    Will return the index of the first non-zero element; and will return np.nan if no non-zero elements exist
+    It doesn't seem like any existing functions satesfied this need
+    https://stackoverflow.com/questions/16243955/numpy-first-occurrence-of-value-greater-than-existing-value
+    :param x:
+    :return:
+    """
+    non_zero = np.where(x)[0]
+    return np.int(non_zero[0]) if len(non_zero) else np.nan
+
+def get_random_state(seed=12345):
+    rs = RandomState(MT19937(SeedSequence(seed)))
+    return rs
+
+def numpy_mode(x):
+    """
+    compute the mode of a numpy array
+    :param x:
+    :return:
+    """
+    values, counts = np.unique(x, return_counts=True)
+    return values[np.argmax(counts)]
+
```

### Comparing `matviz-0.0.7/matviz/helpers_graphing.py` & `matviz-0.0.8/matviz/helpers_graphing.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,42 +11,45 @@
 import collections
 import datetime
 from datetime import datetime as dt
 import pickle
 import glob
 import mpld3
 import time # used in tic() toc()
+import copy
 
 
 # # use these in notebooks
 # %load_ext autoreload
 # %autoreload 2
 # %matplotlib
 
 # should we filter warnings by default? probably not
 # import warnings
 # warnings.filterwarnings('ignore')
 
 # import directly a bunch of useful functions from matplotlib and numpy
 import matplotlib.patches as patches
 from matplotlib.pyplot import plot, hist, figure, clf, cla, xlabel, ylabel, xlim, ylim, \
-                              gcf, gca, close, title, legend, grid, bar, suptitle, show,\
-                              xticks, yticks, hist2d, pcolor, yscale, xscale, axis, pcolor,\
-                              contour, colorbar, scatter, boxplot, savefig
+                              gcf, gca, sca, close, title, legend, grid, bar, suptitle, show,\
+                              xticks, yticks, hist2d, pcolor, pcolormesh, yscale, xscale, axis,\
+                              contour, colorbar, scatter, boxplot, savefig, tight_layout,\
+                              text
 
 from numpy import mean, log10, log, sqrt, power, linspace, sin, cos, tan,\
                         arcsin, arccos, arctan, inf, nan
 
+from math import pi
 from random import random as rand
 
 # load in all the specialized functions.
 from .viz import *
 from .etl import *
 from .histogram_utils import nhist, ndhist
-
+from . import cbrt_scale
 
 # If you get JSON serilization errors because of zoomplot, then you might need this
 # python -m pip install --user "git+https://github.com/javadba/mpld3@display_fix"
 def zoom_plot(enable = True):
     if enable:
         mpld3.enable_notebook()
     else:
@@ -66,15 +69,15 @@
     print("%"+ str(round(100*cnt/N)) + ", " + str(cnt) + "/" + str(N))
 
 def return_pnct(cnt,N):
     return ("%"+ str(round(100*cnt/N)) + ", " + str(cnt) + "/" + str(N))
 
 
 # display the status every so often
-def count_helper(cnt, S, freq=10, pcnt=False):
+def count_helper(cnt, S=1, freq=10, pcnt=False):
     if pcnt:
         freq = np.round(S * freq / 100)
 
     if cnt % freq == 0:
         if pcnt:
             print(str(100.0 * cnt / S) + "% complete")
         else:
@@ -84,31 +87,31 @@
     """
     Homemade version of matlab tic function
     modified by Lansey for python3 from->
     http://stackoverflow.com/questions/5849800/tic-toc-functions-analog-in-python
 
     """
     global startTime_for_tictoc
-    startTime_for_tictoc = time.time()
+    startTime_for_tictoc = time.perf_counter()
 
 def toc():
     """
     Homemade version of matlab toc function
     modified by Lansey for python3 from->
     http://stackoverflow.com/questions/5849800/tic-toc-functions-analog-in-python
 
     """
     if not startTime_for_tictoc:
         print('hey you never hit start')
     else:
         if 'startTime_for_tictoc' in globals():
-            print("Elapsed time is " + str(time.time() - startTime_for_tictoc) + " seconds.")
+            print("Elapsed time is " + str(time.perf_counter() - startTime_for_tictoc) + " seconds.")
         else:
             print("Toc: start time not set")
-        return time.time() - startTime_for_tictoc
+        return time.perf_counter() - startTime_for_tictoc
 
 
 def silent_toc():
     """
     Homemade version of matlab toc function
     modified by Lansey for python3 from->
     http://stackoverflow.com/questions/5849800/tic-toc-functions-analog-in-python
@@ -121,10 +124,24 @@
         import time
         if 'startTime_for_tictoc' in globals():
             return time.time() - startTime_for_tictoc
         else:
             return None
 
 
+def xticklabels(all_lbl):
+    gca().set_xticklabels(all_lbl)
+def yticklabels(all_lbl):
+    gca().set_yticklabels(all_lbl)
+
+
+def nhist_multi(cur, **varargs):
+    n = int(np.ceil(np.sqrt(len(cur))))
+    for cnt, k in enumerate(cur.keys()):
+        subplotter(n, n, cnt)
+        nhist(cur[k], **varargs)
+        title(k)
+    tight_layout()
+
 # set some nice defaults for plotting
 plt.rcParams["figure.figsize"] = [12, 9]
 plt.rcParams['image.cmap'] = 'viridis'
```

### Comparing `matviz-0.0.7/matviz/histogram_utils.py` & `matviz-0.0.8/matviz/histogram_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,14 +125,16 @@
 
         if normalize in ['frac','proportion','prop','percent']:
             normalize_flag = True
             # if normalize in ['frac']:
             fracylabel_flag = True
             # else:
             #     fracylabel_flag = False
+        elif normalize in {'number', 'none'}:
+            normalize_flag = False
         else:
             normalize_flag = normalize
 
 
     elif normalize == False:
         normalize_flag = multiple_flag
     else: # must be set to none specifically
@@ -280,28 +282,29 @@
     # clean up things a bit
     plt.grid(False)
 
     plt.gca().spines['top'].set_visible(False)
     plt.gca().spines['right'].set_visible(False)
 
 
-    return ax, N,bins_in
+    return ax, N, bins_in
 
 
 
 def ndhist(x, y=None, log_colorbar_flag=False, maxx=None, maxy=None, minx=None, miny=None,
                                     int_bins_flag=False, int_bins_flagx=False, int_bins_flagy=False,
                                     exclude_extremes=False,
                                     normy=False, normx = False,
                                     fx=1.5, fy=1.5, std_times=4, f=None,
                                     smooth = False,
                                     markertype=None,
                                     normr = False,
                                     colors = 'none',
-                                    levels=False):
+                                    levels=False,
+                                    level_color=None):
     """
 
     :param x: the x values of data, or y values if no y is passed, or complex numbers where x=real and y=imag
     :param y: the y values of data, leave blank for timeseries without x
     :param log_colorbar_flag: boolean, set the colorbar scale to log
     :param maxx: the maximum x axis limit
     :param maxy: the maximum y axis limit
@@ -344,42 +347,14 @@
         return norms
 
     class nf(float):
         def __repr__(self):
             s = f'{self:.1f}'
             return f'{self:.0f}' if s[-1] == '0' else s
 
-    # this version of the algorithm is very fast - but will artificially include differences in colors
-    # could rewrite it somehow to use this and be faster:
-    # etl.start_and_ends(diff(counts_ordered) < 0)
-    def counts_to_pcnts_fast(counts):
-        flat_counts = flatten(counts)
-        # sort the counts,            [in reverese]
-        idxs = np.argsort(flat_counts)[::-1]
-        idxs_undo = np.argsort(idxs)
-        # flip from greatest to smallest
-        counts_ordered = flat_counts[idxs]
-        # this is counting the contents of the bins in order from fullest to least full
-        counts_summed = np.cumsum(counts_ordered)
-        # convert the counts to a percent of the total N items histogrammed
-        flat_norms = 100 * counts_summed / sum(counts_ordered)
-
-        # get unique values of number of elements in each bin
-        unique_values = np.unique(counts_ordered)
-
-        # for each unique bin value, avg the pcnts and assign that avg for every index with that value
-        for value in unique_values:
-            indices_to_avg = np.where(counts_ordered == value)
-            avg_pcnt = np.mean(flat_norms[indices_to_avg])
-            flat_norms[indices_to_avg] = avg_pcnt
-
-        # reverse the operations to get back to our original orders and shape
-        norms_unsorted = flat_norms[idxs_undo]
-        norms = unflatten(norms_unsorted, counts)
-        return norms
 
     if colors == 'none':
         if levels:
             if type(levels) == bool:
                 colors = plt.cm.Greens
             else:
                 colors = 'gray'
@@ -478,23 +453,25 @@
         to_plot = counts_to_pcnts_fast(to_plot)
         dsx = np.diff(bins_x)[1]
         dsy = np.diff(bins_y)[1]
 
         bx = np.append(bins_x[1:-1] - dsx / 2, np.array([bins_x[-2] + dsx / 2]))
         by = np.append(bins_y[1:-1] - dsy / 2, np.array([bins_y[-2] + dsy / 2]))
 
-        if type(levels) == bool:
+        if isinstance(levels, bool):
 
             plt.contourf(bx, by, to_plot, cmap=colors, levels=100)
         else:
             # fig, ax = plt.subplots()
             ax = plt.gca()
             CS = plt.contour(bx, by, to_plot, colors=colors, levels=levels)
             CS.levels = [nf(val) for val in CS.levels]
             ax.clabel(CS, CS.levels, inline=True, fmt='%r %%', fontsize=10, colors = 'k')
+            if level_color is not None:
+                plt.contourf(bx, by, to_plot, levels=[0, level_color['level']], cmap=level_color['cmap'])
 
         # fig, ax = plt.subplots()
 
     else:
         plt.pcolor(bins_x, bins_y, to_plot, cmap=colors)
 
     plt.xlim(np.array(bins_x)[[1, -2]])
@@ -503,15 +480,42 @@
     if markertype != None:
         plt.plot(x, y, markertype)
 
     # plt.axis('tight')
     return counts, bins_x, bins_y
 
 
-
+# this version of the algorithm is very fast - but will artificially include differences in colors
+# could rewrite it somehow to use this and be faster:
+# etl.start_and_ends(diff(counts_ordered) < 0)
+def counts_to_pcnts_fast(counts):
+    flat_counts = flatten(counts)
+    # sort the counts,            [in reverese]
+    idxs = np.argsort(flat_counts)[::-1]
+    idxs_undo = np.argsort(idxs)
+    # flip from greatest to smallest
+    counts_ordered = flat_counts[idxs]
+    # this is counting the contents of the bins in order from fullest to least full
+    counts_summed = np.cumsum(counts_ordered)
+    # convert the counts to a percent of the total N items histogrammed
+    flat_norms = 100 * counts_summed / sum(counts_ordered)
+
+    # get unique values of number of elements in each bin
+    unique_values = np.unique(counts_ordered)
+
+    # for each unique bin value, avg the pcnts and assign that avg for every index with that value
+    for value in unique_values:
+        indices_to_avg = np.where(counts_ordered == value)
+        avg_pcnt = np.mean(flat_norms[indices_to_avg])
+        flat_norms[indices_to_avg] = avg_pcnt
+
+    # reverse the operations to get back to our original orders and shape
+    norms_unsorted = flat_norms[idxs_undo]
+    norms = unflatten(norms_unsorted, counts)
+    return norms
 
 def choose_bins(X, min_bins=10, max_bins=175, bin_factor=1.5, sameBinsFlag=False, std_times=4, minx=None, maxx=None,
                 int_bins_flag=None, exclude_extremes=True):
 
     # Uses Scott's normal reference rule to select the number of bins
     # https://en.wikipedia.org/wiki/Histogram#Scott's_normal_reference_rule
     # If multiple sets of data are passed then it makes sensible choices
@@ -559,56 +563,59 @@
             maxS[k]=maxx;
             if maxx>np.min(Values):
                 maxS[k]=maxx
             else: # ooh man, even your smallest value is bigger than your max
                 maxS[k]=np.max(Values)
                 # warning(['user parameter maxx=' num2str(maxX) ' override since it put all your data out of bounds']);
     #
+
     # if intbins(k)
     #     maxS(k)=round(maxS(k))+.5;
     #     minS(k)=round(minS(k))-.5; # subtract 1/2 to make the bin peaks appear on the numbers.
     # end
 
     # need the isData boolean to so you are only looking at the ones that actually have some data
     x_min = np.min(minS)
     x_max = np.max(maxS)
 
 # % note that later there will be a bit added to maxS of SXRange
 # % This below is to get estimates for appropriate binsizes
 # totalRange=diff(SXRange); % if the range is zero, then make it eps instead.
 
 
-    total_range = x_max-x_min
+    total_range = x_max - x_min
+
     if int_bins_flag is not None:
         int_bins = [int_bins_flag for x in X]
     else:
         int_bins = [isdiscrete(x) for x in X]
 
-    bin_widths = [3.5*np.std(x)/(bin_factor*np.power(len(x),1.0/3)) for x in X]
+    # scotts choice bin width
+    bin_widths = [3.5 * np.std(x) / (bin_factor * np.power(len(x), 1.0 / 3)) for x in X]
 
   # Instate a mininum and maximum number of bins
     num_bins = [1.0 * total_range/bin_width for bin_width in bin_widths] # Approx number of bins
-
+    num_bins = np.round(num_bins)
     for k in range(S):
         if num_bins[k]<min_bins: # if this will imply less than 10 bins
-            bin_widths[k]=total_range/(min_bins) # set so there are ten bins
+            num_bins[k] = min_bins
+            bin_widths[k] = total_range / (min_bins) # set so there are ten bins
+
         if num_bins[k]>max_bins: # if there would be more than 175 bins (way too many)
-            bin_widths[k]=total_range/max_bins
-#   Check if it is intbins, becase then:
-        if int_bins[k]:# binwidth must be an integer, and it must be at least 1
-            bin_widths[k] = np.max([np.round(bin_widths[k]),1])
-
-        # if numBins>=30 && proportionFlag
-        #     warning('it might not make sense to use ''proportion'' here since you have so many bins')
-        # end
-        # if numBins>=100 && (proportionFlag || numberFlag)
-        #     warning('it might make sense to use ''pdf'' here since you have so many bins')
-        # end
+            num_bins[k] = max_bins
+            bin_widths[k]=total_range / max_bins
+
+        # This will make the span of bins have edges that go up to and include the extreme-most data
+        bin_widths[k] = total_range / num_bins[k] + eps * 100
+
+#   Check if it is intbins, because then:
+        if int_bins[k]: # binwidth must be an integer, and it must be at least 1
+            bin_widths[k] = np.max([np.round(bin_widths[k]), 1])
+            x_min = np.floor(x_min)
 
-    n_bins=[1.0 * total_range/w for w in bin_widths]
 
 ##   if there is enough space to plot them, then plot vertical lines.
 ## 30 bins is arbitrarily chosen to be the number after which there are
 ## vertical lines plotted by default
     # if n_bins(k)<30:
     #     vertLinesArray(k)=1;
     # else
@@ -626,30 +633,30 @@
 
 ##  resize bins to be multiples of each other - or equal
 # sameBinsFlag will make all bin sizes the same.
 
     # Note that in all these conditions the largest histogram bin width
     # divides evenly into the smaller bins. This way the data will line up and
     # you can easily visually compare the values in different bins
-    if sameBinsFlag: # if 'same' is passed then make them all equal to the average reccomended size
+    if sameBinsFlag: # if 'same' is passed then make them all equal to the average recommended size
         only_bin_width = np.mean(bin_widths)
-        bin_widths=[only_bin_width for w in bin_widths]
+        if int_bins_flag:
+            only_bin_width = np.round(only_bin_width)
+        bin_widths=[only_bin_width] * len(bin_widths)
     else: # the bins will be different if neccesary
         for k in range(len(X)):
     #       The 'ceil' rather than 'round' is supposed to make sure that the
     #       ratio is at lease 1 (divisor at least 2).
             bin_widths[k]=big_bin_width/np.ceil(big_bin_width/bin_widths[k])
 
-
     # SXRange(2) = SXRange(2)+max(binWidth)
     if exclude_extremes:
-        bins = [np.arange(x_min,x_max+big_bin_width,w) for w in bin_widths]
+        bins = [np.arange(x_min, x_max + big_bin_width, w) for w in bin_widths]
     else:
-        bins = [np.concatenate([[-np.inf],np.arange(x_min,x_max+big_bin_width,w), [np.inf]]) for w in bin_widths]
-
+        bins = [np.concatenate([[-np.inf], np.arange(x_min, x_max + big_bin_width, w), [np.inf]]) for w in bin_widths]
 
     return bins, bin_widths
 
 
 def dictify_cols2(df):
     return df.groupby(df.columns[0])[df.columns[1]].apply(lambda w: w.values).to_dict()
```

### Comparing `matviz-0.0.7/matviz/viz.py` & `matviz-0.0.8/matviz/viz.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,34 +12,43 @@
 import numpy as np
 import datetime
 from datetime import datetime as dt
 
 # std library
 from itertools import chain
 
+import math
+import sys
+from queue import PriorityQueue
+import pandas as pd
+
 # typing
 from typing import List, Dict, Union, Any, Iterable
 
 from scipy import stats
 import seaborn as sns
 from .etl import nan_smooth
 from .etl import round_time
+from scipy import interpolate
 
 
 # mini function to change a [a, b] into [[a,b]] for use in the for loop later
 def list_ize(w):
-    if hasattr(w[0], "__len__"):
-        return w
+    if len(w) > 0:
+        if hasattr(w[0], "__len__"):
+            return w
+        else:
+            return [w]
     else:
-        return [w]
+        return []
 
 
 
 
-def plot_range(events, color='#0093e7', y_offset='none', height='none', zorder=None, **varargs):
+def plot_range(events, color='#0093e7', y_offset='none', height='none', zorder=None, alpha=0.5, **varargs):
     """
 
     :param events: x positions where the range should be plotted
     :param color:
     :param y_offset:
     :param height:
     :return:
@@ -53,15 +62,15 @@
 
     to_label = 'none'
     # Fill registered cur_event times
     for cur_event in events:
         plt.fill_between([cur_event[0], cur_event[1]],
                          [height + y_offset, height + y_offset],
                          [y_offset, y_offset],
-                         color=color, alpha=0.5, zorder=zorder, label=to_label, **varargs)
+                         color=color, alpha=alpha, zorder=zorder, label=to_label, **varargs)
         # make sure only one legend item appears for this event series
         to_label = '_nolegend_'
 
 
 
 
 def plot_range_idx(t, events, **varargs):
@@ -86,31 +95,30 @@
     plot_range(event_times, **varargs)
 
 
 
 def plot_cdf(data, *args, **kargs):
     x = sorted(data)
     y = 100 * np.arange(len(data)) / len(data)
-    print(kargs)
     plt.plot(x, y, *args, **kargs)
     plt.ylim([0,100])
 
 
 
 
 def set_fontsize(f_size=15):
     ax = plt.gca()
     [w.set_fontsize(f_size) for w in ([ax.title, ax.xaxis.label, ax.yaxis.label] +
                                                     ax.get_xticklabels() +
                                                     ax.get_yticklabels())]
     return ax
 
 
-def print_fig_fancy(fpathh, dpi=300):
-    plt.savefig(fpathh, dpi=dpi, facecolor=[0, 0, 0, 0])
+def print_fig_fancy(fpathh, dpi=300, **kwargs):
+    plt.savefig(fpathh, dpi=dpi, facecolor=[0, 0, 0, 0], **kwargs)
 
 
 def make_title(title_str,format=False):
 
     if title_str:
 
         lower_case_words = {'in','the','a','and','of'}
@@ -165,14 +173,23 @@
         plt.plot(x, m*np.array(x) + b,**line_styles)
 
 
 # plot complex numbers in an arg and diagram
 def cplot(z, *args, **kargs):
     plot(np.real(z), np.imag(z), *args, **kargs)
 
+
+def cplot_circle(z_center, r):
+    t = np.linspace(0, 2 * np.pi, 100)
+    z = r * np.exp(1j * t) + z_center
+    cplot(z)
+
+def ctext(z, *args, **kargs):
+    plt.text(np.real(z), np.imag(z), *args, **kargs)
+
 def cscatter(z, *args, **kargs):
     scatter(np.real(z), np.imag(z), *args, **kargs)
 
 # add a bulls-eye to the graph, polar grid lines
 def polar_grid(lw=1, r=False, linecolor='.3', style=':', nrings=2, nrays = 6):
     ax = plt.gca()
     axis('equal')
@@ -197,116 +214,170 @@
     cur_plt = cplot(np.array(to_plot), style, color=linecolor, lw=lw)
     xlim(ex)
     ylim(yy)
     return cur_plt
 
 
 # plot a diagonal line with x=y to see if your predictions are biased
-def plot_diag(lw=1, color='.5'):
+def plot_diag(lw=1, color='.5', reverse=False):
     ax = plt.gca()
     ex = ax.get_xlim()
     yy = ax.get_ylim()
     if np.diff(ex)[0] > np.diff(yy)[0]:
         y = yy
         x = yy
     else:
         y = ex
         x = ex
-    plt.plot(x, y, '--', color=color, lw=lw)
+
+    if reverse:
+        x = np.flip(x)
+    plt.plot(x, y, '--', color=color, lw=lw, label='_nolegend_')
 
 # plot a horizontal line, or a vertical line
-def plot_zero(lw=1, lineheight=0, linecolor='.5', style='--', axx='x'):
+def plot_zero(lineheight=0, axx='x', **kwargs):
+
+    if len(kwargs) == 0:
+        kwargs = {'color' : '.5',
+                    'linestyle' : '--',
+                    'lw' : 1,
+                    'label': '_nolegend_'
+                    }
+
     ax = plt.gca()
     if axx == 'x':
         ex = ax.get_xlim()
         x = ex
         y = [lineheight, lineheight]
     elif axx == 'y':
         yy = ax.get_ylim()
         x = [lineheight, lineheight]
         y = yy
     else:
         raise Exception("you can't plot zero on no axis!")
 
-    return plt.plot(x,y,style, color=linecolor, lw=lw)
+    return plt.plot(x,y, **kwargs)
+    # return plt.plot(x,y,style, lw=lw, **kwargs)
 
 def plot_axes(color='.5'):
-    plot_zero(axx='x', linecolor=color)
-    plot_zero(axx='y', linecolor=color)
+    plot_zero(axx='x', color=color)
+    plot_zero(axx='y', color=color)
 
 
 def plot_pin(x, y, color='k'):
     """
     Plot a pin at a specific point on the x axis
     :param x: position of the pin on the x axis
     :param y: height of the pin
     :param color: color of the line and marker
     :return:
     """
     plot([x, x], [0, y], linewidth=3, color=color)
     plot([x], [y], 'o', color=color, markersize=10)
 
 
-def bar_centered(y,**kwargs):
+def bar_centered(y, **kwargs):
 #     its like a regular bar plot, except that it is centered on 1:N integers
     x = np.arange(len(y))+1
-    h = plt.bar(x,y,align='center',**kwargs)
+    h = plt.bar(x, y, align='center', **kwargs)
     plt.xticks(x)
     return h
 
 
+def errorb(cur_series, serror=True):
+    """
+    Plot mean and standard deviation/standard error, for items in a pandas series.
+    boxplot
+    :param cur_series:
+    :param serror: if false then the STD will be used for error bar height instead  of standard error
+    :return:
+    """
+    means = cur_series.apply(np.nanmean)
+    errors = cur_series.apply(np.nanstd)
+    if serror:
+        errors = errors / np.sqrt(len(errors))
+
+    x_pos = np.arange(len(cur_series)) + 1
+    bar(x_pos, means,
+        yerr=errors,
+        align='center',
+        alpha=0.5,
+        color='gray',
+        capsize=4)
+
+    ax = gca()
+    ax.set_xticks(x_pos)
+    ax.set_xticklabels(cur_series.index)
+    format_axis_date()
+
+
+def subplotter_auto(n, ii, **kwargs):
+    #     automatically select the right number of subplots for n items
+    y = int(np.ceil(np.sqrt(n)))
+    x = int(np.ceil(n / y))
+    subplotter(x, y, ii, **kwargs)
+
 
-def subplotter(x, y, n, xlbl=None, ylbl=None):
+def subplotter(x, y=None, nth=None, xlbl=None, ylbl=None):
     """
+    a subplotter function that works like the matlab one does but with index starting at 0
     :param x: number of rows
     :param y: number of columns
-    :param n: order, if you pass a list then it spans multiple rows or columns
+    :param nth: order, if you pass a list then it spans multiple rows or columns
     :param xlbl: xlabel, if you want it to appear way on the bottom
     :param ylbl: ylabel, if you want it to appear way on the left only
     :return:
     """
-    # a subplotter function that works like the matlab one does but with index starting at 0
+
+    # allow you to enter input like (220) instead of x=2, y=2, nth =0
+    if x > 99:
+        nth = int(x % 10)
+        y = int((x - nth) % 100)
+        x = int((x - y) / 100)
+        y = int(y / 10)
+
     kwargs = {}
-    if type(n) != int:
+    if type(nth) != int:
         # note special case y == 1, where rowspan should be used
-        if len(n) > y:
+        if len(nth) > y:
             kwargs = {'colspan': y,
-                      'rowspan': len(n) / y}
+                      'rowspan': len(nth) / y}
             if int(kwargs['rowspan']) != kwargs['rowspan']:
                 raise Exception("this isn't supported yet")
             else:
                 kwargs['rowspan'] = int(kwargs['rowspan'])
 
         else:
-            if n[1] == n[0] + 1 and y > 1:
-                kwargs = {'colspan': len(n)}
+            if nth[1] == nth[0] + 1 and y > 1:
+                kwargs = {'colspan': len(nth)}
             else:
-                kwargs = {'rowspan': len(n)}
+                kwargs = {'rowspan': len(nth)}
 
-        n = n[0]
+        nth = nth[0]
     tupp = (x, y)
     cnt = 0
     for ii in range(tupp[0]):
         for jj in range(tupp[1]):
-            if cnt==n:
+            if cnt==nth:
                 ax = plt.subplot2grid(tupp, (ii, jj), **kwargs)
                 if jj == 0:
                     if ylbl:
                         ylabel(ylbl)
+
                 if ii + 1 == x:
                     if xlbl is not None:
                         xlabel(xlbl)
 
 
                 return ax
             cnt+=1
 
 
 
-    raise Exception("You have only " + str(x*y) + " subplots, but you asked for the " + str(n) + "'th")
+    raise Exception("You have only " + str(x*y) + " subplots, but you asked for the " + str(nth) + "'th")
 
 
 def pop_all():
     '''
     bring all the figures hiding in the background to the foreground
     useful when using ipython in the terminal
     '''
@@ -682,21 +753,50 @@
 
     # fix titles so they all appear
     plt.tight_layout()
     # if legend_outside:
     #     gca().legend(loc='center left', bbox_to_anchor=(1, 0.5), framealpha=0.0)
 
 def xylim(w):
+    """
+    Sets x and y limits to be w[0], w[1]
+    if w is a single number then axes are set to -w, w
+    :param w: 
+    :return:
+    """
+    if not hasattr(w, '__len__'):
+        w = [-w, w]
     xlim(w)
     ylim(w)
 
 def xyscale(w):
     plt.xscale(w)
     plt.yscale(w)
 
+def axis_robust(AX):
+    """
+    change the axis limits, but only change one at a time, without changing any of the others
+    :param AX:
+    :return:
+
+    For example, if you want only to set the lower x limit to zero but not change anything else
+    axis_robust([0, None, None, None])
+    """
+    AX_orig = axis()
+    for ii in range(4):
+        if AX[ii] is None:
+            AX[ii] = AX_orig[ii]
+    axis(AX)
+
+def xlim_robust(AX):
+    axis_robust([AX, *ylim()])
+
+def ylim_robust(AX):
+    axis_robust([*xlim(), AX])
+
 
 def set_axis_ticks_pctn(cur_axis = 'x'):
     fmt = '%.0f%%'  # Format you want the ticks, e.g. '40%'
     ticker_obj = matplotlib.ticker.FormatStrFormatter(fmt)
     if cur_axis.lower() == 'x':
         cur_axis_h = gca().xaxis
     elif cur_axis.lower() == 'y':
@@ -829,24 +929,151 @@
     """
 
     y_score = np.concatenate([y1, y2])
     y_true = np.concatenate([np.zeros(len(y1)), np.ones(len(y2))])
 
     return plot_ROC(y_true, y_score)
 
+def plot_ROC_hist(y_true, y_score):
+    y_true = np.array(y_true)
+    y_score = np.array(y_score)
+    return nhist({'true': y_score[y_true], 'false': y_score[~y_true]}, normalize='number')
 
-def plot_ROC(y_true, y_score):
+def plot_ROC(y_true, y_score, c='k'):
 
     I = np.logical_not(np.isnan(y_score))
     y_true = y_true[I]
     y_score = y_score[I]
 
     fpr, tpr, _ = roc_curve(y_true, y_score)
     cur_auc = auc(fpr, tpr)
-    plot(fpr, tpr, 'k')
+    plot(fpr, tpr, c)
     plot_diag()
     xylim([-.01, 1.01])
     plt.xlabel('False Positive Rate')
     plt.ylabel('True Positive Rate')
     plt.title('ROC Curve, AUC = ' + '{:.2f}'.format(cur_auc))
     nicefy()
     return cur_auc
+
+
+def jitter(xx, yy, maxn=4, xscale=None):
+    """
+    in case two point appear at the same value, the jitter function will make
+    them appear slightly separated from each other so you can see the real
+    number of points at a given location.
+    
+    :param xx: 
+    :param yy:
+    :param maxn: the maximum number of dots wide
+    :param exact: if you want to jitter exactly
+    :return:
+    """
+
+    if xscale is None:
+        # split 50 percent of a bar width 1 by the max number of elements to fit
+        xscale = 0.5 / maxn
+
+
+    def get_bins(yy, bin_width):
+        """
+        Get the bins if you know the bin_width
+        Then center it
+        :param yy:
+        :param bin_width:
+        :return:
+        """
+        bins = np.arange(min(yy), max(yy) + bin_width, bin_width)
+        # print(bins)
+        # bins = bins - (max(bins) - max(yy)) / 2
+        return bins
+
+
+    def get_bin_width(yy, maxn, n_iter=5):
+        """
+        Get the right bin width, do a binary search on histogram bin width
+        checking various bin widths until you've found one where at most 'n' items fall in one bin
+        if everything is equal then the maxn parameter doesn't matter
+        todo: handle the case where y values are equal more elegantly
+        :param yy:
+        :return:
+        """
+
+        # if you know the bin width - what is the most that fall in one bin
+        get_max_per_bin = lambda yy, bin_width: np.max(np.histogram(yy, bins=get_bins(yy, bin_width))[0])
+
+        # initialize bin width options to be the most and least it could be
+        if np.std(yy) == 0:
+            bin_width = 1
+        else:
+            yy_sort = sorted(yy)
+            bin_width_min = np.min(np.diff(yy_sort))
+            bin_width_max = yy_sort[-1] - yy_sort[0]
+            for cnt in range(n_iter):
+                bin_width = (bin_width_max + bin_width_min) / 2
+                max_per_bin = get_max_per_bin(yy, bin_width)
+                if max_per_bin >= maxn:
+                    bin_width_max = bin_width
+                else:
+                    bin_width_min = bin_width
+
+        return bin_width
+
+    if len(yy) < 2:
+        # if there is only one point, then you don't need to jitter it
+        return xx
+    else:
+        xx = np.array(xx).astype(float)
+
+        bin_width = get_bin_width(yy, maxn, n_iter=5)
+        bins = get_bins(yy, bin_width)
+
+        idxs = np.digitize(yy, bins, right=True)
+        for bin_idx in range(len(bins)):
+            I = idxs == bin_idx
+            n = sum(I)
+            push = -(n - 1) / 2 # so it will be centered if there is only one.
+            xx[I] = xx[I] + xscale * (push + np.arange(n))
+
+    return xx
+
+def interp_plot(x, y, *args, **kargs):
+    """
+    if you don't have a lot of x data points, then pchip interpolate to make the graphs look smooth
+    :param x: x
+    :param y: y
+    :param n: number of data points to interpolate with
+    :return:
+    """
+
+    y = np.array(y)
+    x = np.array(x)
+
+    if len(x) == 0:
+        return
+
+    date_flag = type(x[0]) == pd._libs.tslibs.timestamps.Timestamp
+    if date_flag:
+        x = np.array([w.value for w in x])
+
+    n = 400
+    I = np.logical_not(pd.isnull(y))
+
+    x = x[I]
+    y = y[I]
+
+    x_i = np.linspace(np.min(x), np.max(x), n)
+
+    f = interpolate.PchipInterpolator(x, y)
+    y_i = f(x_i)
+
+    if date_flag:
+        x_i = np.array([pd.Timestamp(w) for w in x_i])
+
+    plot(x_i, y_i, *args, **kargs)
+
+    return x_i, y_i
+
+
+
+
+
```

### Comparing `matviz-0.0.7/matviz.egg-info/PKG-INFO` & `matviz-0.0.8/matviz.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: matviz
-Version: 0.0.7
+Version: 0.0.8
 Summary: matviz: matrix data visualization
 Home-page: https://github.com/JLansey/matviz
+Download-URL: https://github.com/JLansey/matviz
 Author: Jonathan Lansey
 Author-email: jonathan@lansey.net
 Maintainer: Jonathan Lansey
 Maintainer-email: jonathan@lansey.net
 License: BSD (3-clause)
-Download-URL: https://github.com/JLansey/matviz
-Description: MatViz is a library for making nice looking and useful graphics in Python. It is built on top of `matplotlib <https://matplotlib.org/>`_ and closely integrated with `numpy <https://numpy.org/>`_ and `pandas <https://pandas.pydata.org/>`_ data structures.
-        It also pulls from and is inspired by `seaborn <https://https://seaborn.pydata.org/>`_
-        Here is some of the functionality that matviz offers:
-        - A histogram function that compares multiple distributions with default settings to maximize utility
-        - A 2D histogram function with fun tricks like smoothing and plotting timeseries data
-        - Specialized support for using complex numbers in place of x and y (z = x + 1j * y)
-        - Taking any figure and making it look nicer than the matplotlib defaults
-        - Streamgraph implementation with lots of additional features, based on stackedplot
-        - Lots of plotting functions to import by default and make the coding environment similar to Matlab.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
+License-File: LICENSE
+
+MatViz is a library for making nice looking and useful graphics in Python. It is built on top of `matplotlib <https://matplotlib.org/>`_ and closely integrated with `numpy <https://numpy.org/>`_ and `pandas <https://pandas.pydata.org/>`_ data structures.
+It also pulls from and is inspired by `seaborn <https://https://seaborn.pydata.org/>`_
+Here is some of the functionality that matviz offers:
+- A histogram function that compares multiple distributions with default settings to maximize utility
+- A 2D histogram function with fun tricks like smoothing and plotting timeseries data
+- Specialized support for using complex numbers in place of x and y (z = x + 1j * y)
+- Taking any figure and making it look nicer than the matplotlib defaults
+- Streamgraph implementation with lots of additional features, based on stackedplot
+- Lots of plotting functions to import by default and make the coding environment similar to Matlab.
```

### Comparing `matviz-0.0.7/setup.py` & `matviz-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 DISTNAME = 'matviz'
 MAINTAINER = 'Jonathan Lansey'
 MAINTAINER_EMAIL = 'jonathan@lansey.net'
 URL = 'https://github.com/JLansey/matviz'
 LICENSE = 'BSD (3-clause)'
 DOWNLOAD_URL = 'https://github.com/JLansey/matviz'
-VERSION = 'v0.0.7'
+VERSION = 'v0.0.8'
 
 INSTALL_REQUIRES = [
     'numpy>=1.9.3',
     'scipy>=0.14.0',
     'pandas>=0.15.2',
     'matplotlib>=1.4.3',
     'seaborn>=0.5.1',
@@ -39,14 +39,15 @@
 ]
 
 CLASSIFIERS = [
     'Intended Audience :: Science/Research',
     'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.9',
     'License :: OSI Approved :: BSD License',
     'Topic :: Scientific/Engineering :: Visualization',
     'Topic :: Multimedia :: Graphics',
     'Operating System :: POSIX',
     'Operating System :: Unix',
     'Operating System :: MacOS'
 ]
```

