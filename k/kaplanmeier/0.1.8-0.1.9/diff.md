# Comparing `tmp/kaplanmeier-0.1.8.tar.gz` & `tmp/kaplanmeier-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaplanmeier-0.1.8.tar", last modified: Mon Jun  6 08:05:08 2022, max compression
+gzip compressed data, was "kaplanmeier-0.1.9.tar", last modified: Mon May  8 20:02:54 2023, max compression
```

## Comparing `kaplanmeier-0.1.8.tar` & `kaplanmeier-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-06-06 08:05:08.725280 kaplanmeier-0.1.8/
--rw-rw-rw-   0        0        0     1107 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/LICENSE
--rw-rw-rw-   0        0        0       86 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4223 2022-06-06 08:05:08.721709 kaplanmeier-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3612 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2022-06-06 08:05:08.667978 kaplanmeier-0.1.8/kaplanmeier/
--rw-rw-rw-   0        0        0      988 2022-06-06 08:04:56.000000 kaplanmeier-0.1.8/kaplanmeier/__init__.py
-drwxrwxrwx   0        0        0        0 2022-06-06 08:05:08.713698 kaplanmeier-0.1.8/kaplanmeier/data/
--rw-rw-rw-   0        0        0     1619 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/kaplanmeier/data/survival_example_data.txt
--rw-rw-rw-   0        0        0     1195 2022-06-06 07:54:17.000000 kaplanmeier-0.1.8/kaplanmeier/examples.py
-drwxrwxrwx   0        0        0        0 2022-06-06 08:05:08.718740 kaplanmeier-0.1.8/kaplanmeier/helpers/
--rw-rw-rw-   0        0        0        0 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/kaplanmeier/helpers/__init__.py
--rw-rw-rw-   0        0        0     1736 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/kaplanmeier/helpers/savefig.py
--rw-rw-rw-   0        0        0    13098 2022-06-06 08:04:35.000000 kaplanmeier-0.1.8/kaplanmeier/kaplanmeier.py
-drwxrwxrwx   0        0        0        0 2022-06-06 08:05:08.702673 kaplanmeier-0.1.8/kaplanmeier.egg-info/
--rw-rw-rw-   0        0        0     4223 2022-06-06 08:05:07.000000 kaplanmeier-0.1.8/kaplanmeier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2022-06-06 08:05:08.000000 kaplanmeier-0.1.8/kaplanmeier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-06-06 08:05:07.000000 kaplanmeier-0.1.8/kaplanmeier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-06-06 08:05:08.000000 kaplanmeier-0.1.8/kaplanmeier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-06-06 08:05:08.000000 kaplanmeier-0.1.8/kaplanmeier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-06-06 08:05:08.725667 kaplanmeier-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1393 2022-06-05 14:49:15.000000 kaplanmeier-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:02:54.184417 kaplanmeier-0.1.9/
+-rw-rw-rw-   0        0        0     1107 2022-06-05 14:49:15.000000 kaplanmeier-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0       86 2022-06-05 14:49:15.000000 kaplanmeier-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4182 2023-05-08 20:02:54.183452 kaplanmeier-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3612 2023-05-08 19:58:14.000000 kaplanmeier-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-08 20:02:54.169459 kaplanmeier-0.1.9/kaplanmeier/
+-rw-rw-rw-   0        0        0      988 2023-05-08 18:36:51.000000 kaplanmeier-0.1.9/kaplanmeier/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:02:54.180427 kaplanmeier-0.1.9/kaplanmeier/data/
+-rw-rw-rw-   0        0        0     1619 2022-06-05 14:49:15.000000 kaplanmeier-0.1.9/kaplanmeier/data/survival_example_data.txt
+-rw-rw-rw-   0        0        0     1210 2023-05-08 20:02:29.000000 kaplanmeier-0.1.9/kaplanmeier/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:02:54.182424 kaplanmeier-0.1.9/kaplanmeier/helpers/
+-rw-rw-rw-   0        0        0        0 2022-06-05 14:49:15.000000 kaplanmeier-0.1.9/kaplanmeier/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1736 2022-06-05 14:49:15.000000 kaplanmeier-0.1.9/kaplanmeier/helpers/savefig.py
+-rw-rw-rw-   0        0        0    13643 2023-05-08 20:01:20.000000 kaplanmeier-0.1.9/kaplanmeier/kaplanmeier.py
+drwxrwxrwx   0        0        0        0 2023-05-08 20:02:54.179468 kaplanmeier-0.1.9/kaplanmeier.egg-info/
+-rw-rw-rw-   0        0        0     4182 2023-05-08 20:02:53.000000 kaplanmeier-0.1.9/kaplanmeier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-05-08 20:02:54.000000 kaplanmeier-0.1.9/kaplanmeier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-08 20:02:53.000000 kaplanmeier-0.1.9/kaplanmeier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 20:02:53.000000 kaplanmeier-0.1.9/kaplanmeier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-08 20:02:53.000000 kaplanmeier-0.1.9/kaplanmeier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-08 20:02:54.184417 kaplanmeier-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1393 2022-06-05 14:49:15.000000 kaplanmeier-0.1.9/setup.py
```

### Comparing `kaplanmeier-0.1.8/LICENSE` & `kaplanmeier-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kaplanmeier-0.1.8/PKG-INFO` & `kaplanmeier-0.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: kaplanmeier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create survival curves using kaplanmeier, the log-rank test and making plots.
 Home-page: https://erdogant.github.io/kaplanmeier
-Download-URL: https://github.com/erdogant/kaplanmeier/archive/0.1.8.tar.gz
+Download-URL: https://github.com/erdogant/kaplanmeier/archive/0.1.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,15 +39,17 @@
 ```bash
 pip install kaplanmeier
 ```
 
 #### Import kaplanmeier package
 
 ```python
-import kaplanmeier import km
+
+import kaplanmeier as km
+
 ```
 # 
 
 
 ### [Documentation pages](https://erdogant.github.io/kaplanmeier/)
 
 On the [documentation pages](https://erdogant.github.io/kaplanmeier/) you can find detailed information about the working of the ``kaplanmeier`` with many examples. 
@@ -104,9 +104,7 @@
 <hr>
 
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: kaplanmeier Version: 0.1.8 Summary: Create survival
+Metadata-Version: 2.1 Name: kaplanmeier Version: 0.1.9 Summary: Create survival
 curves using kaplanmeier, the log-rank test and making plots. Home-page: https:
 //erdogant.github.io/kaplanmeier Download-URL: https://github.com/erdogant/
-kaplanmeier/archive/0.1.8.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # kaplanmeier [!
-[Python](https://img.shields.io/pypi/pyversions/kaplanmeier)](https://
-img.shields.io/pypi/pyversions/kaplanmeier) [![PyPI Version](https://
-img.shields.io/pypi/v/kaplanmeier)](https://pypi.org/project/kaplanmeier/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/kaplanmeier/blob/master/LICENSE) [![Github Forks](https://
-img.shields.io/github/forks/erdogant/kaplanmeier.svg)](https://github.com/
-erdogant/kaplanmeier/network) [![GitHub Open Issues](https://img.shields.io/
-github/issues/erdogant/kaplanmeier.svg)](https://github.com/erdogant/
-kaplanmeier/issues) [![Project Status](http://www.repostatus.org/badges/latest/
-active.svg)](http://www.repostatus.org/#active) [![Downloads](https://
-pepy.tech/badge/kaplanmeier/month)](https://pepy.tech/project/kaplanmeier/) [!
-[Downloads](https://pepy.tech/badge/kaplanmeier)](https://pepy.tech/project/
-kaplanmeier) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https:
-//erdogant.github.io/kaplanmeier/)   ``kaplanmeier`` is a Python package to
-compute the kaplan meier curves, log-rank test, and make the plots. # **â­ï¸
-Star this repo if you like it â­ï¸** # #### Install kaplanmeier from PyPI
-```bash pip install kaplanmeier ``` #### Import kaplanmeier package ```python
-import kaplanmeier import km ``` # ### [Documentation pages](https://
-erdogant.github.io/kaplanmeier/) On the [documentation pages](https://
-erdogant.github.io/kaplanmeier/) you can find detailed information about the
-working of the ``kaplanmeier`` with many examples.
+kaplanmeier/archive/0.1.9.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # kaplanmeier [![Python](https://img.shields.io/pypi/
+pyversions/kaplanmeier)](https://img.shields.io/pypi/pyversions/kaplanmeier) [!
+[PyPI Version](https://img.shields.io/pypi/v/kaplanmeier)](https://pypi.org/
+project/kaplanmeier/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/kaplanmeier/blob/master/LICENSE) [!
+[Github Forks](https://img.shields.io/github/forks/erdogant/kaplanmeier.svg)]
+(https://github.com/erdogant/kaplanmeier/network) [![GitHub Open Issues](https:
+//img.shields.io/github/issues/erdogant/kaplanmeier.svg)](https://github.com/
+erdogant/kaplanmeier/issues) [![Project Status](http://www.repostatus.org/
+badges/latest/active.svg)](http://www.repostatus.org/#active) [![Downloads]
+(https://pepy.tech/badge/kaplanmeier/month)](https://pepy.tech/project/
+kaplanmeier/) [![Downloads](https://pepy.tech/badge/kaplanmeier)](https://
+pepy.tech/project/kaplanmeier) [![Sphinx](https://img.shields.io/badge/Sphinx-
+Docs-Green)](https://erdogant.github.io/kaplanmeier/)   ``kaplanmeier`` is a
+Python package to compute the kaplan meier curves, log-rank test, and make the
+plots. # **â­ï¸ Star this repo if you like it â­ï¸** # #### Install
+kaplanmeier from PyPI ```bash pip install kaplanmeier ``` #### Import
+kaplanmeier package ```python import kaplanmeier as km ``` # ### [Documentation
+pages](https://erdogant.github.io/kaplanmeier/) On the [documentation pages]
+(https://erdogant.github.io/kaplanmeier/) you can find detailed information
+about the working of the ``kaplanmeier`` with many examples.
 ===============================================================================
 ### Examples # * [Example: Create Kaplan meier plot](https://
 erdogant.github.io/kaplanmeier/pages/html/Examples.html)
 [https://github.com/erdogant/kaplanmeier/blob/master/docs/figs/fig2.png]
 # * [Example: Remove the Confidence intervals from plot](https://
 erdogant.github.io/kaplanmeier/pages/html/Examples.html#custom-colormap)
 [https://github.com/erdogant/kaplanmeier/blob/master/docs/figs/fig1.png]
```

### Comparing `kaplanmeier-0.1.8/README.md` & `kaplanmeier-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 ```bash
 pip install kaplanmeier
 ```
 
 #### Import kaplanmeier package
 
 ```python
-import kaplanmeier import km
+
+import kaplanmeier as km
+
 ```
 # 
 
 
 ### [Documentation pages](https://erdogant.github.io/kaplanmeier/)
 
 On the [documentation pages](https://erdogant.github.io/kaplanmeier/) you can find detailed information about the working of the ``kaplanmeier`` with many examples.
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 pepy.tech/badge/kaplanmeier/month)](https://pepy.tech/project/kaplanmeier/) [!
 [Downloads](https://pepy.tech/badge/kaplanmeier)](https://pepy.tech/project/
 kaplanmeier) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https:
 //erdogant.github.io/kaplanmeier/)   ``kaplanmeier`` is a Python package to
 compute the kaplan meier curves, log-rank test, and make the plots. # **â­ï¸
 Star this repo if you like it â­ï¸** # #### Install kaplanmeier from PyPI
 ```bash pip install kaplanmeier ``` #### Import kaplanmeier package ```python
-import kaplanmeier import km ``` # ### [Documentation pages](https://
+import kaplanmeier as km ``` # ### [Documentation pages](https://
 erdogant.github.io/kaplanmeier/) On the [documentation pages](https://
 erdogant.github.io/kaplanmeier/) you can find detailed information about the
 working of the ``kaplanmeier`` with many examples.
 ===============================================================================
 ### Examples # * [Example: Create Kaplan meier plot](https://
 erdogant.github.io/kaplanmeier/pages/html/Examples.html)
 [https://github.com/erdogant/kaplanmeier/blob/master/docs/figs/fig2.png]
```

### Comparing `kaplanmeier-0.1.8/kaplanmeier/__init__.py` & `kaplanmeier-0.1.9/kaplanmeier/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     fit,
 	plot,
 	example_data,
 )
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 # module level doc-string
 __doc__ = """
 kaplanmeier - This packages computes the log-rank P-value and computes survival curves based on kaplan meier.
 ===============================================================================================================
 
 **kaplanmeier**
```

### Comparing `kaplanmeier-0.1.8/kaplanmeier/data/survival_example_data.txt` & `kaplanmeier-0.1.9/kaplanmeier/data/survival_example_data.txt`

 * *Files identical despite different names*

### Comparing `kaplanmeier-0.1.8/kaplanmeier/examples.py` & `kaplanmeier-0.1.9/kaplanmeier/examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # %% Examples
-from kaplanmeier import kaplanmeier as km
+import kaplanmeier as km
 # Example data
 df = km.example_data()
 # Fit
 results = km.fit(df['time'], df['Died'], df['group'])
 # Plot
-km.plot(results, title='Custom title text')
+km.plot(results, title='Custom title text', legend=0, fontsize=4)
 km.plot(results, cmap='Set1', cii_lines=True, cii_alpha=0.05)
 km.plot(results, cmap=[(1, 0, 0),(0, 0, 1)])
-km.plot(results, cmap='Set1', methodtype='custom', title=None)
+km.plot(results, cmap='Set1', methodtype='custom', title=None, legend=4)
 results['logrank_P']
 results['logrank_Z']
 
 # %%
 
 # Import library
 import kaplanmeier as km
```

### Comparing `kaplanmeier-0.1.8/kaplanmeier/helpers/savefig.py` & `kaplanmeier-0.1.9/kaplanmeier/helpers/savefig.py`

 * *Files identical despite different names*

### Comparing `kaplanmeier-0.1.8/kaplanmeier/kaplanmeier.py` & `kaplanmeier-0.1.9/kaplanmeier/kaplanmeier.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,19 +98,31 @@
     out['logrank_Z']=test_statistic
     out['logrank']=out_lr
     out['labx']=labx
     out['uilabx']=uilabx
     out['time_event']=time_event
     out['censoring']=censoring
 
-    return(out)
+    return out
 
 
 # %% Make plot
-def plot(out, fontsize=12, savepath='', width=10, height=6, cmap='Set1', cii_alpha=0.05, cii_lines='dense', methodtype='lifeline', title=None, full_ylim=False, y_percentage=False):
+def plot(out,
+         fontsize=12,
+         savepath='',
+         width=10,
+         height=6,
+         cmap='Set1',
+         cii_alpha=0.05,
+         cii_lines='dense',
+         methodtype='lifeline',
+         title=None,
+         full_ylim=False,
+         y_percentage=False,
+         legend=1):
     """Make plot.
 
     Parameters
     ----------
     out : dict
         Results from the fit function.
     fontsize : int (default: 12)
@@ -145,14 +157,20 @@
         Implementation type.
         'dense'   (dense/filled lines)
         'line'
          None  (no lines)
     title : str (default: None)
         In case of None, the logrank P-values is shown.
         Title of the plot.
+    legend : int, default: 0
+        0 : No legend
+        1 : 'upper right'
+        2 : 'upper left'
+        3 : 'lower left'
+        4 : 'lower right'
 
     Returns
     -------
     None.
 
     Examples
     --------
@@ -182,69 +200,77 @@
     Param['savepath'] = savepath
     labx=out['labx']
 
     # Combine data and gather class labels
     data = np.vstack((out['time_event'], out['censoring'])).T
 
     # Make colors and legend-names for class-labels
-    [class_colors, classlabel] = make_class_color_names(data, out['labx'], out['uilabx'], cmap=cmap)
+    class_colors, classlabel = make_class_color_names(data, out['labx'], out['uilabx'], cmap=cmap)
 
     if methodtype=='lifeline':
         # Init
         kmf_all=[]
 
         # Startup figure
         fig = plt.figure(figsize=(Param['width'], Param['height']))
         ax = fig.add_subplot(111)
         if full_ylim:
             ax.set_ylim([0.0, 1.05])
         if y_percentage:
             ax.yaxis.set_major_formatter(PercentFormatter(1.0))
-        plt.title(title)
+        ax.set_title(title)
 
         # Compute KM survival coordinates per class
         if cii_lines=='dense':
             cii_lines=False
         if cii_lines=='line':
             cii_lines=True
-        if cii_lines=='' or cii_lines==None or cii_alpha==None:
+        if (cii_lines=='') or (cii_lines is None) or (cii_alpha is None):
             cii_lines=False
             cii_alpha=0
 
         for i in range(0, len(out['uilabx'])):
             kmf = KaplanMeierFitter()
             idx=np.where(labx==out['uilabx'][i])[0]
             # Fit
             kmf.fit(out['time_event'][idx], event_observed=out['censoring'][idx], label=classlabel[i], ci_labels=None, alpha=(1 - cii_alpha))
             # Plot
-            kmf.plot(ax=ax, ci_force_lines=cii_lines, color=class_colors[i], show_censors=True)
+            kmf.plot(ax=ax, ci_force_lines=cii_lines, color=class_colors[i], show_censors=True, legend=0)
             # Store
             kmf_all.append(kmf.fit(out['time_event'][idx], event_observed=out['censoring'][idx], label=classlabel[i], ci_labels=None, alpha=(1 - cii_alpha)))
 
         add_at_risk_counts(*kmf_all, ax=ax)
 
         ax.tick_params(axis='x', length=15, width=1, direction='out', labelsize=Param['fontsize'])
         ax.tick_params(axis='y', length=15, width=1, direction='out', labelsize=Param['fontsize'])
         ax.spines['bottom'].set_position(['outward', Param['fontsize']])
         ax.spines['left'].set_position(['outward', Param['fontsize']])
         #    ax.rc('font', size= Param['fontsize'])   # controls default text sizes
         #    ax.rc('axes',  labelsize = Param['fontsize'])  # fontsize of the x and y labels
+        if legend>0: ax.legend(loc=legend, fontsize=10)
 
         if Param['savepath']!='':
             savefig(fig, Param['savepath'])
 
     if (methodtype=='custom') or (methodtype is None):
         # Compute KM survival coordinates per class
         for i in range(0, len(out['uilabx'])):
             idx = np.where(labx==out['uilabx'][i])[0]
             tmpdata = data[idx, :].tolist()
             KMcoord[i] = compute_coord(tmpdata)
 
         # Plot KM survival lines
-        _plotkm(KMcoord, classlabel, cmap=class_colors, width=Param['width'], height=Param['height'], fontsize=Param['fontsize'], title=title)
+        _plotkm(KMcoord,
+                classlabel,
+                cmap=class_colors,
+                width=Param['width'],
+                height=Param['height'],
+                fontsize=Param['fontsize'],
+                title=title,
+                legend=legend)
 
 
 # %% Compute coordinates (custom implementation)
 def compute_coord(survtimes):
     """Compute coordinates."""
     h_coords=[]
     v_coords=[]
@@ -282,15 +308,15 @@
             break
 
     newsurv=newsurv[newsurv.index(j) + 1:]
     return (newsurv, y, h_coords, v_coords, lost)
 
 
 # %% Show surival plot (custom implementation)
-def _plotkm(KMcoord, uilabx, cmap='Set1', fontsize=10, width=10, height=6, title=None):
+def _plotkm(KMcoord, uilabx, cmap='Set1', fontsize=10, width=10, height=6, title=None, legend=1):
     """Surival plot."""
     # Get unique colors for class-labels
     if 'str' in str(type(cmap)):
         class_colors=sns.color_palette(cmap, len(KMcoord))
     else:
         class_colors=cmap
 
@@ -333,15 +359,15 @@
         ax.spines['right'].set_visible(False)
         ax.spines['left'].set_linewidth(1)
         ax.spines['bottom'].set_linewidth(1)
         ax.spines['left'].set_bounds(0, 100)
         ax.xaxis.set_ticks_position('bottom')
         ax.yaxis.set_ticks_position('left')
 
-    plt.legend()
+    if legend>0: ax.legend(loc=legend, fontsize=10)
     plt.title(title)
     plt.ylim(0, 105)
     plt.xlim(0,)
     plt.show()
 
 
 # %% Make class colors
```

### Comparing `kaplanmeier-0.1.8/kaplanmeier.egg-info/PKG-INFO` & `kaplanmeier-0.1.9/kaplanmeier.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: kaplanmeier
-Version: 0.1.8
+Version: 0.1.9
 Summary: Create survival curves using kaplanmeier, the log-rank test and making plots.
 Home-page: https://erdogant.github.io/kaplanmeier
-Download-URL: https://github.com/erdogant/kaplanmeier/archive/0.1.8.tar.gz
+Download-URL: https://github.com/erdogant/kaplanmeier/archive/0.1.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,15 +39,17 @@
 ```bash
 pip install kaplanmeier
 ```
 
 #### Import kaplanmeier package
 
 ```python
-import kaplanmeier import km
+
+import kaplanmeier as km
+
 ```
 # 
 
 
 ### [Documentation pages](https://erdogant.github.io/kaplanmeier/)
 
 On the [documentation pages](https://erdogant.github.io/kaplanmeier/) you can find detailed information about the working of the ``kaplanmeier`` with many examples. 
@@ -104,9 +104,7 @@
 <hr>
 
 
 ### Maintainer
 * Erdogan Taskesen, github: [erdogant](https://github.com/erdogant)
 * Contributions are welcome.
 * If you wish to buy me a <a href="https://www.buymeacoffee.com/erdogant">Coffee</a> for this work, it is very appreciated :)
-
-
```

#### html2text {}

```diff
@@ -1,36 +1,35 @@
-Metadata-Version: 2.1 Name: kaplanmeier Version: 0.1.8 Summary: Create survival
+Metadata-Version: 2.1 Name: kaplanmeier Version: 0.1.9 Summary: Create survival
 curves using kaplanmeier, the log-rank test and making plots. Home-page: https:
 //erdogant.github.io/kaplanmeier Download-URL: https://github.com/erdogant/
-kaplanmeier/archive/0.1.8.tar.gz Author: Erdogan Taskesen Author-email:
-erdogant@gmail.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE # kaplanmeier [!
-[Python](https://img.shields.io/pypi/pyversions/kaplanmeier)](https://
-img.shields.io/pypi/pyversions/kaplanmeier) [![PyPI Version](https://
-img.shields.io/pypi/v/kaplanmeier)](https://pypi.org/project/kaplanmeier/) [!
-[License](https://img.shields.io/badge/license-MIT-green.svg)](https://
-github.com/erdogant/kaplanmeier/blob/master/LICENSE) [![Github Forks](https://
-img.shields.io/github/forks/erdogant/kaplanmeier.svg)](https://github.com/
-erdogant/kaplanmeier/network) [![GitHub Open Issues](https://img.shields.io/
-github/issues/erdogant/kaplanmeier.svg)](https://github.com/erdogant/
-kaplanmeier/issues) [![Project Status](http://www.repostatus.org/badges/latest/
-active.svg)](http://www.repostatus.org/#active) [![Downloads](https://
-pepy.tech/badge/kaplanmeier/month)](https://pepy.tech/project/kaplanmeier/) [!
-[Downloads](https://pepy.tech/badge/kaplanmeier)](https://pepy.tech/project/
-kaplanmeier) [![Sphinx](https://img.shields.io/badge/Sphinx-Docs-Green)](https:
-//erdogant.github.io/kaplanmeier/)   ``kaplanmeier`` is a Python package to
-compute the kaplan meier curves, log-rank test, and make the plots. # **â­ï¸
-Star this repo if you like it â­ï¸** # #### Install kaplanmeier from PyPI
-```bash pip install kaplanmeier ``` #### Import kaplanmeier package ```python
-import kaplanmeier import km ``` # ### [Documentation pages](https://
-erdogant.github.io/kaplanmeier/) On the [documentation pages](https://
-erdogant.github.io/kaplanmeier/) you can find detailed information about the
-working of the ``kaplanmeier`` with many examples.
+kaplanmeier/archive/0.1.9.tar.gz Author: Erdogan Taskesen Author-email:
+erdogant@gmail.com Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3 Description-Content-Type: text/markdown
+License-File: LICENSE # kaplanmeier [![Python](https://img.shields.io/pypi/
+pyversions/kaplanmeier)](https://img.shields.io/pypi/pyversions/kaplanmeier) [!
+[PyPI Version](https://img.shields.io/pypi/v/kaplanmeier)](https://pypi.org/
+project/kaplanmeier/) [![License](https://img.shields.io/badge/license-MIT-
+green.svg)](https://github.com/erdogant/kaplanmeier/blob/master/LICENSE) [!
+[Github Forks](https://img.shields.io/github/forks/erdogant/kaplanmeier.svg)]
+(https://github.com/erdogant/kaplanmeier/network) [![GitHub Open Issues](https:
+//img.shields.io/github/issues/erdogant/kaplanmeier.svg)](https://github.com/
+erdogant/kaplanmeier/issues) [![Project Status](http://www.repostatus.org/
+badges/latest/active.svg)](http://www.repostatus.org/#active) [![Downloads]
+(https://pepy.tech/badge/kaplanmeier/month)](https://pepy.tech/project/
+kaplanmeier/) [![Downloads](https://pepy.tech/badge/kaplanmeier)](https://
+pepy.tech/project/kaplanmeier) [![Sphinx](https://img.shields.io/badge/Sphinx-
+Docs-Green)](https://erdogant.github.io/kaplanmeier/)   ``kaplanmeier`` is a
+Python package to compute the kaplan meier curves, log-rank test, and make the
+plots. # **â­ï¸ Star this repo if you like it â­ï¸** # #### Install
+kaplanmeier from PyPI ```bash pip install kaplanmeier ``` #### Import
+kaplanmeier package ```python import kaplanmeier as km ``` # ### [Documentation
+pages](https://erdogant.github.io/kaplanmeier/) On the [documentation pages]
+(https://erdogant.github.io/kaplanmeier/) you can find detailed information
+about the working of the ``kaplanmeier`` with many examples.
 ===============================================================================
 ### Examples # * [Example: Create Kaplan meier plot](https://
 erdogant.github.io/kaplanmeier/pages/html/Examples.html)
 [https://github.com/erdogant/kaplanmeier/blob/master/docs/figs/fig2.png]
 # * [Example: Remove the Confidence intervals from plot](https://
 erdogant.github.io/kaplanmeier/pages/html/Examples.html#custom-colormap)
 [https://github.com/erdogant/kaplanmeier/blob/master/docs/figs/fig1.png]
```

### Comparing `kaplanmeier-0.1.8/setup.py` & `kaplanmeier-0.1.9/setup.py`

 * *Files identical despite different names*

