# Comparing `tmp/complex_curve_fit_gui-1.1.6.tar.gz` & `tmp/complex_curve_fit_gui-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "complex_curve_fit_gui-1.1.6.tar", last modified: Thu Apr 27 09:44:30 2023, max compression
+gzip compressed data, was "complex_curve_fit_gui-1.1.7.tar", last modified: Mon May  8 00:18:06 2023, max compression
```

## Comparing `complex_curve_fit_gui-1.1.6.tar` & `complex_curve_fit_gui-1.1.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.190835 complex_curve_fit_gui-1.1.6/
--rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.1.6/MANIFEST.in
--rw-r--r--   0 kojo       (501) staff       (20)     9399 2023-04-27 09:44:30.190926 complex_curve_fit_gui-1.1.6/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)     8940 2023-04-27 04:46:22.000000 complex_curve_fit_gui-1.1.6/README.md
--rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-04-27 09:44:30.191215 complex_curve_fit_gui-1.1.6/setup.cfg
--rw-rw-rw-   0 kojo       (501) staff       (20)     1299 2023-04-24 04:40:32.000000 complex_curve_fit_gui-1.1.6/setup.py
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.188503 complex_curve_fit_gui-1.1.6/src/
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.189996 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/
--rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/__init__.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_curvefitgui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    15964 2023-04-27 09:32:17.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_gui.py
--rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_settings.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    16635 2023-04-27 08:22:23.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_tools.py
--rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-04-27 09:42:11.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_version.py
--rw-rw-rw-   0 kojo       (501) staff       (20)    33637 2023-04-27 09:31:48.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_widgets.py
--rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/config.txt
-drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-04-27 09:44:30.190562 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/
--rw-r--r--   0 kojo       (501) staff       (20)     9399 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/PKG-INFO
--rw-r--r--   0 kojo       (501) staff       (20)      582 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/SOURCES.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/dependency_links.txt
--rw-r--r--   0 kojo       (501) staff       (20)       22 2023-04-27 09:44:30.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/top_level.txt
--rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/zip-safe
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 00:18:06.242333 complex_curve_fit_gui-1.1.7/
+-rw-r--r--   0 kojo       (501) staff       (20)       44 2023-04-24 04:46:49.000000 complex_curve_fit_gui-1.1.7/MANIFEST.in
+-rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 00:18:06.242435 complex_curve_fit_gui-1.1.7/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)     9657 2023-05-08 00:07:44.000000 complex_curve_fit_gui-1.1.7/README.md
+-rw-rw-rw-   0 kojo       (501) staff       (20)       79 2023-05-08 00:18:06.242774 complex_curve_fit_gui-1.1.7/setup.cfg
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1299 2023-04-24 04:40:32.000000 complex_curve_fit_gui-1.1.7/setup.py
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 00:18:06.238508 complex_curve_fit_gui-1.1.7/src/
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 00:18:06.241320 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/
+-rw-rw-rw-   0 kojo       (501) staff       (20)      181 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/__init__.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     7155 2023-04-27 04:39:20.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_curvefitgui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    15968 2023-05-07 23:59:53.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_gui.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)     1529 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_settings.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    16715 2023-05-07 23:22:42.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_tools.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)       22 2023-05-08 00:17:22.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_version.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)    32342 2023-04-28 06:02:55.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_widgets.py
+-rw-rw-rw-   0 kojo       (501) staff       (20)      879 2023-01-31 03:12:15.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/config.txt
+drwxr-xr-x   0 kojo       (501) staff       (20)        0 2023-05-08 00:18:06.242049 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/
+-rw-r--r--   0 kojo       (501) staff       (20)    10116 2023-05-08 00:18:06.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/PKG-INFO
+-rw-r--r--   0 kojo       (501) staff       (20)      582 2023-05-08 00:18:06.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-05-08 00:18:06.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 kojo       (501) staff       (20)       22 2023-05-08 00:18:06.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/top_level.txt
+-rw-r--r--   0 kojo       (501) staff       (20)        1 2023-04-24 04:57:58.000000 complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/zip-safe
```

### Comparing `complex_curve_fit_gui-1.1.6/PKG-INFO` & `complex_curve_fit_gui-1.1.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex_curve_fit_gui
-Version: 1.1.6
+Version: 1.1.7
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 - Using `conda` (required for M1 Mac):    
 
       conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
-       `from curvefitgui import curve_fit_gui`
+       `from complex_curve_fit_gui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
        `ydata = np.array([-3.5, -2.4, -1, 0.5, 1.8])`
 4. Call curve_fit_gui:
     - Set first parameter to None to be able to select predefined functions
     - For example: 
 
@@ -71,19 +71,23 @@
  - xlabel : string, optional (default:'x-values')
         x-axis title in the plot
  - ylabel : string, optional (default:'y-values')
         y-axis title in the plot
  - title  : string, optional
         data plot title
  - p0 : array-like, optional
-        initial values for fit parameters, if not specified 1 is used for each parameter
+        initial values for fit parameters, if not specified 1 is used for each parameter, if specified length must be >= number of fit parameters else program crashes upon fit
+ - method : string, optional
+       desired fit method for lmfit model, default is "least squares"
  - showgui : boolean, optional (default=True)
         if True, the gui is shown, otherwise not
  - absolute_sigma : boolean, optional
         see doc-string scipy.optimize.curve_fit()
+ - add : array of tuple, optional
+       add additional data sets, requires format `[(np.array, np.array, string)]` which implies `[(x_data, y_data, label)]`. Multiple datasets can be placed in the array, and method is selectable within gui
  - kwargs
         keyword arguments for compatibility (e.g. you can use sigma to specify the error in y)
 
 ### Return Data
 - The curve fit function returns a tuple with three elements.
        1. Array containing the fit parameters
        2. Array containing the standard error (+/-)
@@ -138,14 +142,19 @@
   - **Customize** Change visual features of the plot such as marker type or color and axis titles ![Customize Button Image](images/customize_scr.png)
   - **Pan and Zoom** Shift and zoom on plot ![Pan and Zoom](images/pan_zoom_scr.png)
   - **Left and Right** Undo and redo actions for shift and zoom ![Undo and Redo](images/arrows_scr.png)
   - **Home** Return to original plot view ![Home](images/home_scr.png)
 10. **FitTextbox:** This textbox is generated if a valid fit is performed. It can be moved by the mouse to any convenient positions in the plot.
 11. **Range Selector** Activates/deactivates the range-selector. The range-selector allows to select a datarange used for fitting. Only datapoints that are within the two vertical dashed lines are considered during fitting. The lines can be moved using the mouse.
 ![Range Selector](images/range_selector_scr.png)
+12. **SELECT DATA** Allows user to switch between plotted dataset and desired fit model
+![select data button](images/select_data.png)
+![select data modal](images/switch_data_modal.png)
+13. **TOGGLE Residual** show/hide residual plot
+![toggle residual](images/toggle_residual.png)
 
 
 
 <!-- To run program
 `python3 curve.py"`
 
 #### For someone looking to expand this code:
```

### Comparing `complex_curve_fit_gui-1.1.6/README.md` & `complex_curve_fit_gui-1.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 - Using `conda` (required for M1 Mac):    
 
       conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
-       `from curvefitgui import curve_fit_gui`
+       `from complex_curve_fit_gui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
        `ydata = np.array([-3.5, -2.4, -1, 0.5, 1.8])`
 4. Call curve_fit_gui:
     - Set first parameter to None to be able to select predefined functions
     - For example: 
 
@@ -57,19 +57,23 @@
  - xlabel : string, optional (default:'x-values')
         x-axis title in the plot
  - ylabel : string, optional (default:'y-values')
         y-axis title in the plot
  - title  : string, optional
         data plot title
  - p0 : array-like, optional
-        initial values for fit parameters, if not specified 1 is used for each parameter
+        initial values for fit parameters, if not specified 1 is used for each parameter, if specified length must be >= number of fit parameters else program crashes upon fit
+ - method : string, optional
+       desired fit method for lmfit model, default is "least squares"
  - showgui : boolean, optional (default=True)
         if True, the gui is shown, otherwise not
  - absolute_sigma : boolean, optional
         see doc-string scipy.optimize.curve_fit()
+ - add : array of tuple, optional
+       add additional data sets, requires format `[(np.array, np.array, string)]` which implies `[(x_data, y_data, label)]`. Multiple datasets can be placed in the array, and method is selectable within gui
  - kwargs
         keyword arguments for compatibility (e.g. you can use sigma to specify the error in y)
 
 ### Return Data
 - The curve fit function returns a tuple with three elements.
        1. Array containing the fit parameters
        2. Array containing the standard error (+/-)
@@ -124,14 +128,19 @@
   - **Customize** Change visual features of the plot such as marker type or color and axis titles ![Customize Button Image](images/customize_scr.png)
   - **Pan and Zoom** Shift and zoom on plot ![Pan and Zoom](images/pan_zoom_scr.png)
   - **Left and Right** Undo and redo actions for shift and zoom ![Undo and Redo](images/arrows_scr.png)
   - **Home** Return to original plot view ![Home](images/home_scr.png)
 10. **FitTextbox:** This textbox is generated if a valid fit is performed. It can be moved by the mouse to any convenient positions in the plot.
 11. **Range Selector** Activates/deactivates the range-selector. The range-selector allows to select a datarange used for fitting. Only datapoints that are within the two vertical dashed lines are considered during fitting. The lines can be moved using the mouse.
 ![Range Selector](images/range_selector_scr.png)
+12. **SELECT DATA** Allows user to switch between plotted dataset and desired fit model
+![select data button](images/select_data.png)
+![select data modal](images/switch_data_modal.png)
+13. **TOGGLE Residual** show/hide residual plot
+![toggle residual](images/toggle_residual.png)
 
 
 
 <!-- To run program
 `python3 curve.py"`
 
 #### For someone looking to expand this code:
```

### Comparing `complex_curve_fit_gui-1.1.6/setup.py` & `complex_curve_fit_gui-1.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_curvefitgui.py` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_curvefitgui.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_gui.py` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,20 +28,20 @@
         We could check here if fitter.model.func is complex, then immediately call fit after initGUI() so that model.result populates 
         """
         self.fitter = afitter
         self.xlabel, self.ylabel = xlabel, ylabel
         self.output = (None, None)
         self.xerrorwarning = settings["XERRORWARNING"]
         self.kwargs = kwargs
+        self.OG_model = self.fitter.model  # original model/ user entered model
         self.initGUI(**kwargs)
         # call fit here if complex
         # if self.fitter.is_complex:
         #     self.fit()
         self.plotwidget.update_plot()
-        self.OG_model = self.fitter.model  # original model/ user entered model
 
     def closeEvent(self, event):
         """needed to properly quit when running in IPython console / Spyder IDE"""
         QtWidgets.QApplication.quit()
 
     def initGUI(self, **kwargs):
         # main GUI proprieties
@@ -336,15 +336,15 @@
                 """
                 return a * np.exp(-x / b) * np.cos(c * x + d) + e
 
             def decaying_oscillation2(x, a, b, c, d, e):
                 """
                 y = a * exp(-x / b)^2 * cos(c * x + d) + e
                 """
-                return a * (np.exp(-x / b) ** 2) * np.cos(c * x + d) + e
+                return a * (np.exp(-(x**2) / b**2)) * np.cos(c * x + d) + e
 
             def euler(x, a):
                 """
                 Euler's
                 y = a * exp(i * x)
                 """
                 return a * (np.exp(1j * (x)))
@@ -357,15 +357,15 @@
                 return a * np.exp(1j * (b * x + c)) + d
 
             self.function_map = {
                 "y = ax + b": linear,
                 "y = a * exp(-x / b) + c": exp_decay,
                 "y = a * cos(b*x + c) + d": cosine_function,
                 "y = a * exp(-x / b) * cos(c * x + d) + e": decaying_oscillation,
-                "y = a * exp(-x / b)^2 * cos(c * x + d) + e": decaying_oscillation2,
+                "y = a * exp(-x^2 / b^2)* cos(c * x + d) + e": decaying_oscillation2,
                 "y = a * exp(i * x)": euler,
                 "y = a * exp(i * (b * w + c)) + d": complex_function,
             }
             """
             Drop down box of functions for curve fit
             """
```

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_settings.py` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_settings.py`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_tools.py` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import inspect
 from dataclasses import dataclass, field
+from sys import stderr
 from typing import Any, List
 import copy
 import numpy as np
 from lmfit import Model
 from scipy import stats
 from scipy.optimize import OptimizeWarning, curve_fit
 
@@ -219,18 +220,29 @@
         )
         # lmfit model result
         self.model_result = result
 
         # process results
         self.fit_is_valid = True
         # print("cov", pcov)
-        stderrors = np.sqrt(np.diag(pcov))
-        for fitpar, value, stderr in zip(self.model.fitpars, popt, stderrors):
-            fitpar.value = value
-            fitpar.sigma = stderr
+        """
+        Standard error only works for least squares method another way to calculate standard error needs
+        to be added here
+        """
+        if pcov.any():
+            stderrors = np.sqrt(np.diag(pcov))
+            for fitpar, value, stderr in zip(
+                self.model.fitpars, popt, stderrors
+            ):
+                fitpar.value = value
+                fitpar.sigma = stderr
+        else:
+            for fitpar, value in zip(self.model.fitpars, popt):
+                fitpar.value = value
+                fitpar.sigma = 0
 
         self.mean_squared_error = sum(((y - self.model.evaluate(x)) / ye) ** 2)
 
         self._create_report()
         return popt, pcov, result
 
     def get_curve(
@@ -321,22 +333,17 @@
         # print(self)
 
     def change_model(self, func, p0, absolute_sigma):
         self.model = self._init_model(func, p0, absolute_sigma)
         # print(self)
 
 
-def curve_fit_wrapper(
-    model, *pargs, p0=None, pF=None, method="slsqp", **kwargs
-):
+def curve_fit_wrapper(model, *pargs, p0=None, pF=None, method, **kwargs):
     """
-    wrapper around the scipy curve_fit() function to allow parameters to be fixed
-    same call signature as the curve_fit() function except for:
-    pF : 1D numpy array of size n, with n the number of fitparameters of the function
-    returns the popt and cov matrices just like the original curve_fit() function
+    wrapper around the lmfit model
     """
 
     # extract arguments of the function func
     __args = inspect.signature(model.func).parameters
     args = [arg.name for arg in __args.values()]
 
     # populate pF (fixed marker) and p0 (param value) to default if not provided in kwargs
@@ -379,16 +386,18 @@
     result = model.lmfit_model.fit(
         pargs[1],
         params,
         x=pargs[0],
         calc_covar=True,
         nan_policy="omit",
         method=method,
-        max_nfev=100000000,
+        max_nfev=1000000000,
     )
+    # print("print", result.params["a"])
+    # print("print", result.params["a"].stderr)
 
     popt = np.array(list(result.best_values.values()))
     # print("cov values", result.covar)
     cov = np.array(result.covar)
     # print("cov values after arrayed", cov)
 
     # rebuild the popt and cov to include fixed parameters
@@ -405,15 +414,14 @@
     # rebuild covariance matrix to include both fixed and optimized pars
     for id in id_fix:
         cov = np.insert(
             cov, id, 0, axis=1
         )  # add zero rows and columns for fixed par
         cov = np.insert(cov, id, 0, axis=0)
 
-    # params here temporarily, in future move lmfit model to fitmodel so that params does not need to be returned here
     return popt, cov, result
 
 
 def value_to_string(name, value, error, fixed):
     def get_exponent(value):
         """returns the exponent as an int generated by the :.e format specifier"""
         deci = 5
```

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/_widgets.py` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         self.layout().addWidget(self.toolbar)
         self.layout().addWidget(self.canvas)
 
         self.resized.connect(
             self.update_plot
         )  # update plot when window is resized to fit plot in window
 
+        # functions to switch to
         def linear(x, a, b):
             """
             linear
             function: ax + b
             """
 
             return a * x + b
@@ -256,55 +257,14 @@
                 self.canvas.xlabel,
                 fontname=settings["TEXT_FONT"],
                 fontsize=settings["TEXT_SIZE"],
             )
         self.canvas.ax2.set_visible(not self.canvas.ax2.get_visible())
         self.canvas.redraw()
 
-    def update_data(self):
-        x = np.array([1, 2, 3])
-        y = np.array([4, 5, 6])
-        self.canvas.ax1.plot(
-            x,
-            y,
-            marker="o",
-            lw=0,
-            label="data2",
-        )
-        self.canvas.ax1.legend()
-        self.canvas.redraw()
-
-        # dialog = QtWidgets.QDialog()
-        # dialog.setWindowTitle("Update Data")
-        # layout = QtWidgets.QVBoxLayout()
-
-        # ind_layout = QtWidgets.QHBoxLayout()
-        # ind_label = QtWidgets.QLabel("Independent Values: ")
-        # self.independent_variable = QtWidgets.QLineEdit()
-        # ind_layout.addWidget(ind_label)
-        # ind_layout.addWidget(self.independent_variable)
-
-        # dep_layout = QtWidgets.QHBoxLayout()
-        # dep_label = QtWidgets.QLabel("Dependent Values: ")
-        # self.dependent_variable = QtWidgets.QLineEdit()
-        # dep_layout.addWidget(dep_label)
-        # dep_layout.addWidget(self.dependent_variable)
-
-        # button = QtWidgets.QPushButton("Update")
-        # # button.clicked.connect(self.re_init_plot)
-
-        # layout.addLayout(ind_layout)
-        # layout.addLayout(dep_layout)
-        # layout.addWidget(button)
-
-        # button.clicked.connect(dialog.close)
-
-        # dialog.setLayout(layout)
-        # dialog.exec_()
-
     def switch_data(self):
         def save_complex_data():
             """
             before switching curve add complex data to a map of label to x data and y data
             Since complex plots y real and imag, xdata is lost in matplotlib
             """
```

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui/config.txt` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui/config.txt`

 * *Files identical despite different names*

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/PKG-INFO` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: complex-curve-fit-gui
-Version: 1.1.6
+Version: 1.1.7
 Summary: GUI for lmfit using matplotlib
 Home-page: https://github.com/boakyeni/data-visualization-and-curve-fitting
 Author: Kojo Nimako
 Author-email: boakyeni@usc.edu
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -31,15 +31,15 @@
 - Using `conda` (required for M1 Mac):    
 
       conda install numpy scipy matplotlib qtpy pyqt && conda install -c conda-forge lmfit
 
 ### Getting Started
 1. If on MacOS M1 a conda environment will be needed
 2. import the gui:
-       `from curvefitgui import curve_fit_gui`
+       `from complex_curve_fit_gui import curve_fit_gui`
 3. define x and y data as 1 dimensional numpy arrays of equal length
        `xdata = np.array([1, 2, 3, 4, 5])`
        `ydata = np.array([-3.5, -2.4, -1, 0.5, 1.8])`
 4. Call curve_fit_gui:
     - Set first parameter to None to be able to select predefined functions
     - For example: 
 
@@ -71,19 +71,23 @@
  - xlabel : string, optional (default:'x-values')
         x-axis title in the plot
  - ylabel : string, optional (default:'y-values')
         y-axis title in the plot
  - title  : string, optional
         data plot title
  - p0 : array-like, optional
-        initial values for fit parameters, if not specified 1 is used for each parameter
+        initial values for fit parameters, if not specified 1 is used for each parameter, if specified length must be >= number of fit parameters else program crashes upon fit
+ - method : string, optional
+       desired fit method for lmfit model, default is "least squares"
  - showgui : boolean, optional (default=True)
         if True, the gui is shown, otherwise not
  - absolute_sigma : boolean, optional
         see doc-string scipy.optimize.curve_fit()
+ - add : array of tuple, optional
+       add additional data sets, requires format `[(np.array, np.array, string)]` which implies `[(x_data, y_data, label)]`. Multiple datasets can be placed in the array, and method is selectable within gui
  - kwargs
         keyword arguments for compatibility (e.g. you can use sigma to specify the error in y)
 
 ### Return Data
 - The curve fit function returns a tuple with three elements.
        1. Array containing the fit parameters
        2. Array containing the standard error (+/-)
@@ -138,14 +142,19 @@
   - **Customize** Change visual features of the plot such as marker type or color and axis titles ![Customize Button Image](images/customize_scr.png)
   - **Pan and Zoom** Shift and zoom on plot ![Pan and Zoom](images/pan_zoom_scr.png)
   - **Left and Right** Undo and redo actions for shift and zoom ![Undo and Redo](images/arrows_scr.png)
   - **Home** Return to original plot view ![Home](images/home_scr.png)
 10. **FitTextbox:** This textbox is generated if a valid fit is performed. It can be moved by the mouse to any convenient positions in the plot.
 11. **Range Selector** Activates/deactivates the range-selector. The range-selector allows to select a datarange used for fitting. Only datapoints that are within the two vertical dashed lines are considered during fitting. The lines can be moved using the mouse.
 ![Range Selector](images/range_selector_scr.png)
+12. **SELECT DATA** Allows user to switch between plotted dataset and desired fit model
+![select data button](images/select_data.png)
+![select data modal](images/switch_data_modal.png)
+13. **TOGGLE Residual** show/hide residual plot
+![toggle residual](images/toggle_residual.png)
 
 
 
 <!-- To run program
 `python3 curve.py"`
 
 #### For someone looking to expand this code:
```

### Comparing `complex_curve_fit_gui-1.1.6/src/complex_curve_fit_gui.egg-info/SOURCES.txt` & `complex_curve_fit_gui-1.1.7/src/complex_curve_fit_gui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

