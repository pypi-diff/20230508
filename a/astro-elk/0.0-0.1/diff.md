# Comparing `tmp/astro-elk-0.0.tar.gz` & `tmp/astro-elk-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-elk-0.0.tar", last modified: Tue May  2 20:30:47 2023, max compression
+gzip compressed data, was "astro-elk-0.1.tar", last modified: Mon May  8 21:38:29 2023, max compression
```

## Comparing `astro-elk-0.0.tar` & `astro-elk-0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:30:47.098407 astro-elk-0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 20:30:47.098407 astro-elk-0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-02 20:30:31.000000 astro-elk-0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:30:47.094407 astro-elk-0.0/astro_elk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-02 20:30:47.000000 astro-elk-0.0/astro_elk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-02 20:30:47.000000 astro-elk-0.0/astro_elk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:30:47.000000 astro-elk-0.0/astro_elk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-02 20:30:47.000000 astro-elk-0.0/astro_elk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-02 20:30:47.000000 astro-elk-0.0/astro_elk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:30:47.098407 astro-elk-0.0/elk/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    21634 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/lightcurve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-02 20:30:31.000000 astro-elk-0.0/elk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-02 20:30:47.098407 astro-elk-0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-02 20:30:31.000000 astro-elk-0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:29.339759 astro-elk-0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 21:38:29.339759 astro-elk-0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-08 21:38:15.000000 astro-elk-0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:29.339759 astro-elk-0.1/astro_elk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-08 21:38:29.000000 astro-elk-0.1/astro_elk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 21:38:29.339759 astro-elk-0.1/elk/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21682 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11306 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-08 21:38:16.000000 astro-elk-0.1/elk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-08 21:38:29.339759 astro-elk-0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-08 21:38:16.000000 astro-elk-0.1/setup.py
```

### Comparing `astro-elk-0.0/elk/ensemble.py` & `astro-elk-0.1/elk/ensemble.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         # return a simple summary table that can be stacked with other clusters
         return Table({'name': [self.identifier], 'location': [self.location], 'radius': [self.radius],
                       'log_age': [self.cluster_age], 'has_data': [self.sectors_available > 0],
                       'n_obs': [self.sectors_available], 'n_good_obs': [self.n_good_obs],
                       'which_sectors_good': [[lc.sector for lc in self.lcs if lc is not None]],
                       'n_failed_download': [self.n_failed_download], 'n_bad_quality': [self.n_bad_quality],
                       'n_scatter_light': [len(self.scattered_light_sectors)],
-                      'scattered_light_sectors': [self.scattered_light_sectors],
+                      'scattered_light_sectors': [self.scattered_light_sectors if len(self.scattered_light_sectors) > 0 else 0],
                       'lc_lens': [[len(lc.corrected_lc) for lc in self.lcs if lc is not None]]})
 
 
 def from_fits(filepath, existing_class=None, **kwargs):
     # if an existing class is not provided then create a new blank one
     if existing_class is None:
         new_ecl = EnsembleLC(identifier="", radius=None, cluster_age=None, output_path=None, **kwargs)
```

### Comparing `astro-elk-0.0/elk/lightcurve.py` & `astro-elk-0.1/elk/lightcurve.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.0/elk/plot.py` & `astro-elk-0.1/elk/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     if fap is not None:
         ax.axhline(fap, color="gold", label=f"False alarm probability ({fap:1.2e})")
 
     # set scales and labels
     ax.set_xscale('log')
     ax.set_xlabel(r'Frequency $[1 / {\rm days}]$')
     ax.set_ylabel('Power')
+    ax.legend()
 
     # save and show if desired
     if save_path is not None:
         plt.savefig(save_path, format='png', bbox_inches="tight")
     if show:
         plt.show()
 
@@ -164,15 +165,15 @@
     # create figure if necessary and add title
     if fig is None or ax is None:
         fig, ax = plt.subplots()
     ax.set_title(title)
 
     # if a period is given then fold based on that period and re-sort
     if fold_period is not None:
-        time = (time - time[0]) % fold_period
+        time = ((time - time[0]) %fold_period)/fold_period
         order = np.argsort(time)
         time = time[order]
         flux = flux[order]
 
     ax.plot(time, flux, color=color, linewidth=linewidth, **kwargs)
 
     ax.set_xlabel(r'Time $\rm [days]$')
```

### Comparing `astro-elk-0.0/elk/stats.py` & `astro-elk-0.1/elk/stats.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.0/elk/utils.py` & `astro-elk-0.1/elk/utils.py`

 * *Files identical despite different names*

### Comparing `astro-elk-0.0/setup.cfg` & `astro-elk-0.1/setup.cfg`

 * *Files identical despite different names*

