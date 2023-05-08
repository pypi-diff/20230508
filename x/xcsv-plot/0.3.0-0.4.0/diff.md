# Comparing `tmp/xcsv_plot-0.3.0.tar.gz` & `tmp/xcsv_plot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsv_plot-0.3.0.tar", max compression
+gzip compressed data, was "xcsv_plot-0.4.0.tar", max compression
```

## Comparing `xcsv_plot-0.3.0.tar` & `xcsv_plot-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot-0.3.0/LICENSE
--rw-r--r--   0        0        0     4529 2023-03-26 19:11:15.830946 xcsv_plot-0.3.0/README.md
--rw-r--r--   0        0        0      714 2023-05-01 16:16:56.047116 xcsv_plot-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    12414 2023-05-01 16:17:15.947364 xcsv_plot-0.3.0/xcsv/plot/__init__.py
--rw-r--r--   0        0        0     5025 2023-03-26 19:11:15.830946 xcsv_plot-0.3.0/xcsv/plot/__main__.py
--rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 xcsv_plot-0.3.0/setup.py
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 xcsv_plot-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4529 2023-03-26 19:11:15.830946 xcsv_plot-0.4.0/README.md
+-rw-r--r--   0        0        0      714 2023-05-08 09:32:58.322763 xcsv_plot-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    15433 2023-05-08 09:33:27.763108 xcsv_plot-0.4.0/xcsv/plot/__init__.py
+-rw-r--r--   0        0        0     5008 2023-05-08 09:32:16.354270 xcsv_plot-0.4.0/xcsv/plot/__main__.py
+-rw-r--r--   0        0        0     5463 1970-01-01 00:00:00.000000 xcsv_plot-0.4.0/setup.py
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 xcsv_plot-0.4.0/PKG-INFO
```

### Comparing `xcsv_plot-0.3.0/LICENSE` & `xcsv_plot-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsv_plot-0.3.0/README.md` & `xcsv_plot-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xcsv_plot-0.3.0/pyproject.toml` & `xcsv_plot-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcsv-plot"
-version = "0.3.0"
+version = "0.4.0"
 description = "Subpackage for plotting extended CSV (XCSV) files"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/paul-breen/xcsv-plot"
 homepage = "https://github.com/paul-breen/xcsv-plot"
 documentation = "https://github.com/paul-breen/xcsv-plot/blob/main/README.md"
```

### Comparing `xcsv_plot-0.3.0/xcsv/plot/__init__.py` & `xcsv_plot-0.4.0/xcsv/plot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # Project: Extended CSV common file format
 # Purpose: Classes to plot data from an extended CSV file
 # Author:  Paul M. Breen
 # Date:    2022-05-13
 ###############################################################################
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 import re
 
 import matplotlib.pyplot as plt
 
 import xcsv
 
@@ -30,14 +30,19 @@
         """
 
         self.fig = None
         self.axs = []
         self.datasets = []
         self.xcol = None
         self.ycol = None
+        self.xlabel = None
+        self.ylabel = None
+        self.title = None
+        self.caption = None
+        self.label_key = None
 
     def get_plot_data_extent(self, datasets, xcol, ycol):
         """
         Get the extent over which the datasets range in data coordinates
 
         A list is returned with the shape [left, right, bottom, top].  This
         can be used for the extent kwarg to imshow().
@@ -58,61 +63,74 @@
         if xcol is None:
             extent = [0, max([len(dataset.data) - 1 for dataset in datasets]), min([dataset.data[ycol].min() for dataset in datasets]), max([dataset.data[ycol].max() for dataset in datasets])]
         else:
             extent = [min([dataset.data[xcol].min() for dataset in datasets]), max([dataset.data[xcol].max() for dataset in datasets]), min([dataset.data[ycol].min() for dataset in datasets]), max([dataset.data[ycol].max() for dataset in datasets])]
 
         return extent
 
-    def setup_data_plot(self, fig, ax, xlabel=None, ylabel=None, caption=None, caption_x=0.1, caption_y=0.02, caption_wrap=True, subplots_adjust_bottom=0.15):
+    def add_figure_title(self, title, title_wrap=True):
         """
-        Setup the data plot
+        Add a title to the figure
 
-        This sets fixed annotations, such as the x- and y-axis labels.
+        :param title: The figure title text
+        :type title: str
+        :param title_wrap: Wrap the title text
+        :type title_wrap: bool
+        """
+
+        self.fig.suptitle(title, wrap=title_wrap)
+
+    def add_figure_caption(self, caption, caption_x=0.1, caption_y=0.02, caption_wrap=True, subplots_adjust_bottom=0.15):
+        """
+        Add a caption to the figure
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
-        :param ax: The axis object
-        :type ax: matplotlib.axes.Axes
-        :param xlabel: The x-axis label text
-        :type xlabel: str
-        :param ylabel: The y-axis label text
-        :type ylabel: str
         :param caption: The figure caption text
         :type caption: str
         :param caption_x: An offset for the caption text in the x-direction
         :type caption_x: float
         :param caption_y: An offset for the caption text in the y-direction
         :type caption_y: float
         :param caption_wrap: Wrap the caption text
         :type caption_wrap: bool
         :param subplots_adjust_bottom: Add space to hold the caption
         :type subplots_adjust_bottom: float
         """
 
-        if caption:
-            fig.text(caption_x, caption_y, caption, wrap=caption_wrap)
-            fig.subplots_adjust(bottom=subplots_adjust_bottom)
+        self.fig.text(caption_x, caption_y, caption, wrap=caption_wrap)
+        self.fig.subplots_adjust(bottom=subplots_adjust_bottom)
+
+    def setup_data_plot(self, ax, xlabel=None, ylabel=None):
+        """
+        Setup the data plot
+
+        This sets fixed annotations, such as the x- and y-axis labels.
+
+        :param ax: The axis object
+        :type ax: matplotlib.axes.Axes
+        :param xlabel: The x-axis label text
+        :type xlabel: str
+        :param ylabel: The y-axis label text
+        :type ylabel: str
+        """
 
         if xlabel:
             ax.set_xlabel(xlabel)
 
         if ylabel:
             ax.set_ylabel(ylabel)
 
-    def plot_data(self, fig, ax, dataset, xcol, ycol, label=None, invert_xaxis=False, invert_yaxis=False, opts={}):
+    def plot_data(self, ax, dataset, xcol, ycol, label=None, invert_xaxis=False, invert_yaxis=False, opts={}):
         """
         Plot the data for the given dataset
 
         * The xcol header label specifies the data series from the dataset's
         data table to be used for the x-axis.
         * The ycol header label specifies the data series from the dataset's
         data table to be used for the y-axis.
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
         :param ax: The axis object
         :type ax: matplotlib.axes.Axes
         :param dataset: The dataset to plot
         :type dataset: XCSV object
         :param xcol: The x-axis data column header label
         :type xcol: str
         :param ycol: The y-axis data column header label
@@ -138,20 +156,18 @@
 
         if invert_yaxis:
             ax.invert_yaxis()
 
         if label:
             ax.legend()
 
-    def plot_data_bg(self, fig, ax, img, img_extent, aspect='auto', alpha=0.5):
+    def plot_data_bg(self, ax, img, img_extent, aspect='auto', alpha=0.5):
         """
         Plot the given image as a background for the data plot
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
         :param ax: The axis object
         :type ax: matplotlib.axes.Axes
         :param img: The image data
         :type img: array-like or PIL image
         :param img_extent: The image data extent as [left, right, bottom, top]
         :type img_extent: list
         :param aspect: The aspect ratio of the image
@@ -190,15 +206,15 @@
                 img = plt.imread(img_path)
 
         if not img_extent:
             # This automatically takes care of inverted x or y axes
             img_extent = [*self.axs[axs_idx].get_xlim(), *self.axs[axs_idx].get_ylim()]
 
         if img is not None:
-            self.plot_data_bg(self.fig, self.axs[axs_idx], img, img_extent)
+            self.plot_data_bg(self.axs[axs_idx], img, img_extent)
 
     def setup_figure_and_axes(self, figsize=None):
         """
         Setup the figure and axes array
 
         If not called directly, then it is called by the plot_datasets()
         function.  If a specific figure size is required, then this function
@@ -211,121 +227,195 @@
         :param figsize: The figure size tuple as (width, height)
         :type figsize: tuple
         """
 
         self.fig = plt.figure(figsize=figsize)
         self.axs.append(self.fig.add_subplot())
 
-    def plot_datasets(self, datasets, fig=None, axs=None, axs_idx=0, xcol=None, ycol=None, xidx=None, yidx=0, xlabel=None, ylabel=None, title=None, title_wrap=True, caption=None, label_key=None, invert_xaxis=False, invert_yaxis=False, show=True, opts={}):
+    def _setup_fallback_figure_and_axes(self, fig=None, axs=None):
         """
-        Plot the data for the given datasets
-
-        Either the xcol and ycol column header labels, or the xidx and yidx
-        column indices, can be specified.  These are mutually exclusive.  They
-        identify the data series from the datasets' data tables to be used for
-        the x- and y-axis data.
-
-        If annotations such as the title and caption, and the label_key,
-        are not specified, then they are taken from XCSV header items
-        (see self.DEFAULTS for details).  If these keys are not present in
-        the header, then an empty string is used instead, effectively leaving
-        them blank.
+        Setup a fallback figure and axes array
 
-        If show is set to False, then custom edits can be made to the plot
-        (e.g. adding extra annotations) before displaying.  Also, if saving
-        the plot to an output file instead of displaying, then set show=False.
+        This calls setup_figure_and_axes() if it hasn't already beeen called
 
-        :param datasets: A list of XCSV objects containing the input datasets
-        :type datasets: list
         :param fig: The figure object
         :type fig: matplotlib.figure.Figure
         :param axs: The axes array
         :type axs: matplotlib.axes.Axes
-        :param axs_idx: The index of the axis object in the axs array
-        :type axs_idx: int
+        """
+
+        if fig:
+            self.fig = fig
+
+        if axs:
+            self.axs = axs
+
+        if not self.fig or not self.axs:
+            self.setup_figure_and_axes()
+
+    def _store_figure_parameters(self, datasets, xcol=None, ycol=None, xidx=None, yidx=0, xlabel=None, ylabel=None, title=None, caption=None, label_key=None):
+        """
+        Store the parameters for the figure
+
+        Either the xcol and ycol column header labels, or the xidx and yidx
+        column indices, can be specified.  These are mutually exclusive.
+
+        :param datasets: A list of XCSV objects containing the input datasets
+        :type datasets: list
         :param xcol: The x-axis data column header label
         :type xcol: str
         :param ycol: The y-axis data column header label
         :type ycol: str
         :param xidx: The x-axis data column index
         :type xidx: int
         :param yidx: The y-axis data column index
         :type yidx: int
         :param xlabel: The x-axis label text
         :type xlabel: str
         :param ylabel: The y-axis label text
         :type ylabel: str
         :param title: The figure title text
         :type title: str
-        :param title_wrap: Wrap the title text
-        :type title_wrap: bool
         :param caption: The figure caption text
         :type caption: str
         :param label_key: The key of a header item in the XCSV header to be
         used as a unique label to identify each data series in the plot legend
         :type label_key: str
-        :param invert_xaxis: Invert the x-axis
-        :type invert_xaxis: bool
-        :param invert_yaxis: Invert the y-axis
-        :type invert_yaxis: bool
-        :param show: Show the plot
-        :type show: bool
-        :param opts: Option kwargs to apply to all plots (e.g., color, marker)
-        :type opts: dict
         """
- 
-        if fig:
-            self.fig = fig
-
-        if axs:
-            self.axs = axs
-
-        if not self.fig or not self.axs:
-            self.setup_figure_and_axes()
 
         self.datasets = datasets
         self.xcol = xcol
         self.ycol = ycol
-        generate_colors = True
+        self.xlabel = xlabel
+        self.ylabel = ylabel
+        self.title = title
+        self.caption = caption
+        self.label_key = label_key
 
         if not title:
-            title = datasets[0].get_metadata_item_value(self.DEFAULTS['title_key'])
+            self.title = datasets[0].get_metadata_item_value(self.DEFAULTS['title_key'])
 
         if not caption:
-            caption = datasets[0].get_metadata_item_value(self.DEFAULTS['caption_key'])
+            self.caption = datasets[0].get_metadata_item_value(self.DEFAULTS['caption_key'])
 
         if not label_key:
-            label_key = self.DEFAULTS['label_key']
+            self.label_key = self.DEFAULTS['label_key']
 
         if not xcol:
             if xidx is not None:
                 self.xcol = datasets[0].data.iloc[:, xidx].name
 
         if not ycol:
             self.ycol = datasets[0].data.iloc[:, yidx].name
 
         if not xlabel:
-            xlabel = self.xcol
+            self.xlabel = self.xcol
 
         if not ylabel:
-            ylabel = self.ycol
+            self.ylabel = self.ycol
+
+    def _add_figure_annotations(self, axs_idx=0):
+        """
+        Add annotations to the figure
+
+        :param axs_idx: The index of the axis object in the axs array
+        :type axs_idx: int
+        """
+
+        self.add_figure_title(self.title)
+        self.add_figure_caption(self.caption)
+        self.setup_data_plot(self.axs[axs_idx], xlabel=self.xlabel, ylabel=self.ylabel)
+
+    def _plot_datasets(self, axs_idx=0, invert_xaxis=False, invert_yaxis=False, opts={}):
+        """
+        Plot the data for the figure datasets
+
+        :param axs_idx: The index of the axis object in the axs array
+        :type axs_idx: int
+        :param invert_xaxis: Invert the x-axis
+        :type invert_xaxis: bool
+        :param invert_yaxis: Invert the y-axis
+        :type invert_yaxis: bool
+        :param opts: Option kwargs to apply to all plots (e.g., color, marker)
+        :type opts: dict
+        """
+
+        generate_colors = True
 
         if 'color' in opts:
             generate_colors = False
 
-        self.fig.suptitle(title, wrap=title_wrap)
-        self.setup_data_plot(self.fig, self.axs[axs_idx], caption=caption, xlabel=xlabel, ylabel=ylabel)
-
-        for i, dataset in enumerate(datasets):
-            label = dataset.get_metadata_item_value(label_key)
+        for i, dataset in enumerate(self.datasets):
+            label = dataset.get_metadata_item_value(self.label_key)
 
             if generate_colors:
                 opts.update({'color': f'C{i}'})
 
-            self.plot_data(self.fig, self.axs[axs_idx], dataset, self.xcol, self.ycol, label=label, invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis, opts=opts)
+            self.plot_data(self.axs[axs_idx], dataset, self.xcol, self.ycol, label=label, invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis, opts=opts)
+
+    def plot_datasets(self, datasets, fig=None, axs=None, axs_idx=0, xcol=None, ycol=None, xidx=None, yidx=0, xlabel=None, ylabel=None, title=None, caption=None, label_key=None, invert_xaxis=False, invert_yaxis=False, show=True, opts={}):
+        """
+        Plot the data for the given datasets
+
+        Either the xcol and ycol column header labels, or the xidx and yidx
+        column indices, can be specified.  These are mutually exclusive.  They
+        identify the data series from the datasets' data tables to be used for
+        the x- and y-axis data.
+
+        If annotations such as the title and caption, and the label_key,
+        are not specified, then they are taken from XCSV header items
+        (see self.DEFAULTS for details).  If these keys are not present in
+        the header, then an empty string is used instead, effectively leaving
+        them blank.
+
+        If show is set to False, then custom edits can be made to the plot
+        (e.g. adding extra annotations) before displaying.  Also, if saving
+        the plot to an output file instead of displaying, then set show=False.
+
+        :param datasets: A list of XCSV objects containing the input datasets
+        :type datasets: list
+        :param fig: The figure object
+        :type fig: matplotlib.figure.Figure
+        :param axs: The axes array
+        :type axs: matplotlib.axes.Axes
+        :param axs_idx: The index of the axis object in the axs array
+        :type axs_idx: int
+        :param xcol: The x-axis data column header label
+        :type xcol: str
+        :param ycol: The y-axis data column header label
+        :type ycol: str
+        :param xidx: The x-axis data column index
+        :type xidx: int
+        :param yidx: The y-axis data column index
+        :type yidx: int
+        :param xlabel: The x-axis label text
+        :type xlabel: str
+        :param ylabel: The y-axis label text
+        :type ylabel: str
+        :param title: The figure title text
+        :type title: str
+        :param caption: The figure caption text
+        :type caption: str
+        :param label_key: The key of a header item in the XCSV header to be
+        used as a unique label to identify each data series in the plot legend
+        :type label_key: str
+        :param invert_xaxis: Invert the x-axis
+        :type invert_xaxis: bool
+        :param invert_yaxis: Invert the y-axis
+        :type invert_yaxis: bool
+        :param show: Show the plot
+        :type show: bool
+        :param opts: Option kwargs to apply to all plots (e.g., color, marker)
+        :type opts: dict
+        """
+
+        self._setup_fallback_figure_and_axes(fig, axs)
+        self._store_figure_parameters(datasets, xcol, ycol, xidx, yidx, xlabel, ylabel, title, caption, label_key)
+        self._add_figure_annotations(axs_idx)
+        self._plot_datasets(axs_idx, invert_xaxis, invert_yaxis, opts)
 
         if show:
             plt.show()
 
     def show(self):
         """
         Display the figure
```

### Comparing `xcsv_plot-0.3.0/xcsv/plot/__main__.py` & `xcsv_plot-0.4.0/xcsv/plot/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
     args = parse_cmdln()
     datasets = get_datasets(args.in_file)
     plotter = xp.Plot()
 
     if args.figsize:
         plotter.setup_figure_and_axes(figsize=args.figsize)
 
-    plotter.plot_datasets(datasets, xidx=args.xidx, yidx=args.yidx, xcol=args.xcol, ycol=args.ycol, xlabel=args.xlabel, ylabel=args.ylabel, title=args.title, title_wrap=True, caption=args.caption, label_key=args.label_key, invert_xaxis=args.invert_xaxis, invert_yaxis=args.invert_yaxis, show=False, opts=args.plot_opts)
+    plotter.plot_datasets(datasets, xidx=args.xidx, yidx=args.yidx, xcol=args.xcol, ycol=args.ycol, xlabel=args.xlabel, ylabel=args.ylabel, title=args.title, caption=args.caption, label_key=args.label_key, invert_xaxis=args.invert_xaxis, invert_yaxis=args.invert_yaxis, show=False, opts=args.plot_opts)
 
     if args.bg_img_path:
         plotter.add_plot_bg(img_path=args.bg_img_path)
 
     if args.out_file:
         plotter.savefig(args.out_file)
     else:
```

### Comparing `xcsv_plot-0.3.0/setup.py` & `xcsv_plot-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['matplotlib>=3.5.2,<4.0.0', 'xcsv>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['xcsv_plot = xcsv.plot.__main__:main']}
 
 setup_kwargs = {
     'name': 'xcsv-plot',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Subpackage for plotting extended CSV (XCSV) files',
     'long_description': "# xcsv-plot\n\nxcsv-plot is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv-plot\n```\n\n## Using the package\n\nXCSV data can be plotted directly, as the data table is a `pandas` table:\n\n```python\ncontent.data.plot(x='time (year) [a]', y='depth (m)')\n```\n\nand of course for more control over the plot, the data can be plotted using `matplotlib`, say.\n\nBut an XCSV file with an [ACDD-compliant](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3) extended header section, and well-annotated column-headers, already provides much of the text needed to make an informative plot, so we can just plot the XCSV file directly from the command line.  This is the purpose of the `xcsv-plot` subpackage.  For example:\n\n```bash\n$ python3 -m xcsv.plot -x 0 -y 1 example.csv\n```\n\nNote here that we're calling `xcsv-plot` as a *module main*.  As a convenience, this invocation is wrapped as a console script when installing the package, hence the following invocation is equivalent:\n\n```bash\n$ xcsv_plot -x 0 -y 1 example.csv\n```\n\nIn addition to using the CLI, the package can be used as a Python library.  The main class is `Plot` which provides methods to plot a given list of datasets (XCSV objects):\n\n```python\nimport xcsv\nimport xcsv.plot as xp\n\nfilenames = ['example1.csv','example2.csv','example3.csv']\ndatasets = []\n\nfor filename in filenames:\n    with xcsv.File(filename) as f:\n        datasets.append(f.read())\n\nplotter = xp.Plot()\nplotter.plot_datasets(datasets, xidx=0, yidx=1)\n```\n\n## Command line usage\n\nCalling the script with the `--help` option will show the following usage:\n\n```bash\n$ python3 -m xcsv.plot --help\nusage: xcsv_plot [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]\n                 [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]\n                 [--invert-y-axis] [--title TITLE] [--caption CAPTION]\n                 [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE] [-b BG_IMG_PATH]\n                 [-o OUT_FILE] [-P PLOT_OPTS] [-S] [-V]\n                 in_file [in_file ...]\n\nplot the given XCSV files\n\npositional arguments:\n  in_file               input XCSV file(s)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -x XIDX, --x-idx XIDX\n                        column index (zero-based) containing values for the\n                        x-axis\n  -X XCOL, --x-column XCOL\n                        column label containing values for the x-axis\n  -y YIDX, --y-idx YIDX\n                        column index (zero-based) containing values for the\n                        y-axis\n  -Y YCOL, --y-column YCOL\n                        column label containing values for the y-axis\n  --x-label XLABEL      text to be used for the plot x-axis label\n  --y-label YLABEL      text to be used for the plot y-axis label\n  --invert-x-axis       invert the x-axis\n  --invert-y-axis       invert the y-axis\n  --title TITLE         text to be used for the plot title\n  --caption CAPTION     text to be used for the plot caption\n  --label-key LABEL_KEY\n                        key of the header item in the extended header section\n                        whose value will be used for the plot legend label\n  -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE\n                        size of the figure (width height)\n  -b BG_IMG_PATH, --background-image BG_IMG_PATH\n                        path to an image to show in the background of the plot\n  -o OUT_FILE, --out-file OUT_FILE\n                        output plot file\n  -P PLOT_OPTS, --plot-options PLOT_OPTS\n                        options for the plot, specified as a simple JSON\n                        object\n  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot\n  -V, --version         show program's version number and exit\n\nExamples\n\nGiven an XCSV file with an ACDD-compliant extended header section, and a single column (at column 0) of data values:\n\n# id: 1\n# title: The title\ndepth (m)\n0.575\n1.125\n2.225\n\nThen the following invocation will plot the only column on the y-axis, with the x-axis the indices of the data points:\n\npython3 -m xcsv.plot input.csv\n\nIf the file also contains a suitable variable for the x-axis:\n\n# id: 1\n# title: The title\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n\nthen the columns to be used for the x- and y-axes can be specified thus:\n\npython3 -m xcsv.plot -x 0 -y 1 input.csv\n```\n\n",
     'author': 'Paul Breen',
     'author_email': 'pbree@bas.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/paul-breen/xcsv-plot',
```

### Comparing `xcsv_plot-0.3.0/PKG-INFO` & `xcsv_plot-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsv-plot
-Version: 0.3.0
+Version: 0.4.0
 Summary: Subpackage for plotting extended CSV (XCSV) files
 Home-page: https://github.com/paul-breen/xcsv-plot
 License: Apache-2.0
 Author: Paul Breen
 Author-email: pbree@bas.ac.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

