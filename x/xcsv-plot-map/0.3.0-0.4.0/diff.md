# Comparing `tmp/xcsv_plot_map-0.3.0.tar.gz` & `tmp/xcsv_plot_map-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcsv_plot_map-0.3.0.tar", max compression
+gzip compressed data, was "xcsv_plot_map-0.4.0.tar", max compression
```

## Comparing `xcsv_plot_map-0.3.0.tar` & `xcsv_plot_map-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot_map-0.3.0/LICENSE
--rw-r--r--   0        0        0     6213 2023-03-27 08:49:05.970225 xcsv_plot_map-0.3.0/README.md
--rw-r--r--   0        0        0      836 2023-05-01 19:20:53.512312 xcsv_plot_map-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    22015 2023-05-01 19:17:05.273533 xcsv_plot_map-0.3.0/xcsv/plot_map/__init__.py
--rw-r--r--   0        0        0     5747 2023-03-27 08:49:05.974225 xcsv_plot_map-0.3.0/xcsv/plot_map/__main__.py
--rw-r--r--   0        0        0     7302 1970-01-01 00:00:00.000000 xcsv_plot_map-0.3.0/setup.py
--rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 xcsv_plot_map-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2018-06-22 07:09:46.422789 xcsv_plot_map-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6371 2023-05-08 09:54:21.071208 xcsv_plot_map-0.4.0/README.md
+-rw-r--r--   0        0        0      836 2023-05-08 09:55:33.016732 xcsv_plot_map-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    24705 2023-05-08 09:55:52.325128 xcsv_plot_map-0.4.0/xcsv/plot_map/__init__.py
+-rw-r--r--   0        0        0     6079 2023-05-08 09:54:21.075208 xcsv_plot_map-0.4.0/xcsv/plot_map/__main__.py
+-rw-r--r--   0        0        0     7462 1970-01-01 00:00:00.000000 xcsv_plot_map-0.4.0/setup.py
+-rw-r--r--   0        0        0     7336 1970-01-01 00:00:00.000000 xcsv_plot_map-0.4.0/PKG-INFO
```

### Comparing `xcsv_plot_map-0.3.0/LICENSE` & `xcsv_plot_map-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xcsv_plot_map-0.3.0/README.md` & `xcsv_plot_map-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
 ```bash
 $ python -m xcsv.plot_map --help
 usage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]
                      [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]
                      [--invert-y-axis] [--title TITLE] [--caption CAPTION]
                      [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]
-                     [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]
+                     [-p PROJECTION] [-m] [-b BG_IMG_PATH] [-o OUT_FILE]
                      [-P PLOT_OPTS] [-S] [-V]
                      in_file [in_file ...]
 
 plot the given XCSV files and locate the data on a map
 
 positional arguments:
   in_file               input XCSV file(s)
@@ -106,14 +106,16 @@
                         whose value will be used for the plot legend label
   -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE
                         size of the figure (width height)
   -p PROJECTION, --map-projection PROJECTION
                         projection to use for displaying the site coordinates
                         on the map (one of the CRS classes provided by
                         Cartopy)
+  -m, --plot-on-map     instead of a plot alongside a site map, show just a
+                        map and plot the coordinate data directly on the map
   -b BG_IMG_PATH, --background-image BG_IMG_PATH
                         path to an image to show in the background of the plot
   -o OUT_FILE, --out-file OUT_FILE
                         output plot file
   -P PLOT_OPTS, --plot-options PLOT_OPTS
                         options for the plot, specified as a simple JSON
                         object
```

### Comparing `xcsv_plot_map-0.3.0/pyproject.toml` & `xcsv_plot_map-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xcsv-plot-map"
-version = "0.3.0"
+version = "0.4.0"
 description = "Subpackage to plot and locate on a map, data from extended CSV (XCSV) files"
 authors = ["Paul Breen <pbree@bas.ac.uk>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/paul-breen/xcsv-plot-map"
 homepage = "https://github.com/paul-breen/xcsv-plot-map"
 documentation = "https://github.com/paul-breen/xcsv-plot-map/blob/main/README.md"
@@ -13,15 +13,15 @@
 ]
 
 [tool.poetry.scripts]
 xcsv_plot_map = "xcsv.plot_map.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-xcsv-plot = "^0.3.0"
+xcsv-plot = "^0.4.0"
 matplotlib = "^3.5.2"
 Cartopy = "^0.21.1"
 shapely = "^2.0.1"
 scipy = "^1.8.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
```

### Comparing `xcsv_plot_map-0.3.0/xcsv/plot_map/__init__.py` & `xcsv_plot_map-0.4.0/xcsv/plot_map/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ###############################################################################
 # Project: Extended CSV common file format
 # Purpose: Classes to plot and locate on a map data from an extended CSV file
 # Author:  Paul M. Breen
 # Date:    2022-05-15
 ###############################################################################
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 
 import os
 import re
 
 import matplotlib.pyplot as plt
 import cartopy.crs as ccrs
 from shapely import geometry
@@ -167,22 +167,20 @@
         elif bbox_test_key in test_dataset.metadata['header']:
             extent = self.get_site_plot_extent_from_bbox(datasets)
         else:
             raise KeyError(f"Cannot calculate map extent as required spatial coordinate keys were not found in the header")
 
         return extent
 
-    def setup_site_plot(self, fig, ax, extent, crs=None, bg_img_name=None, bg_img_resolution='low', coastlines_resolution='10m', add_gridlines=True):
+    def setup_site_plot(self, ax, extent, crs=None, bg_img_name=None, bg_img_resolution='low', coastlines_resolution='10m', add_gridlines=True, draw_gridline_labels=True):
         """
         Setup the site map
 
         This sets fixed properties of the map, such as extent and base map.
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
         :param ax: The axis object
         :type ax: matplotlib.axes.Axes
         :param extent: The geographical bounding box extent for the map
         as [left, right, bottom, top]
         :type extent: list
         :param crs: The CRS for the map.  If not specified, it defaults to
         ccrs.PlateCarree()
@@ -196,36 +194,36 @@
         :param bg_img_resolution: A supported resolution of the background
         image name given in bg_img_name
         :type bg_img_resolution: str
         :param coastlines_resolution: The resolution of the coastlines
         :type coastlines_resolution: str
         :param add_gridlines: Add gridlines to the map
         :type add_gridlines: bool
+        :param draw_gridline_labels: Draw gridline labels on the map
+        :type draw_gridline_labels: bool
         """
 
         if not crs:
             crs = ccrs.PlateCarree()
 
         ax.set_extent(extent, crs=crs)
         ax.coastlines(resolution=coastlines_resolution)
 
         if bg_img_name:
             ax.background_img(name=bg_img_name, resolution=bg_img_resolution)
         else:
             ax.stock_img()
 
         if add_gridlines:
-            ax.gridlines()
+            ax.gridlines(draw_labels=draw_gridline_labels)
 
-    def plot_point_site(self, fig, ax, dataset, xkey='longitude', ykey='latitude', site_key='site', transform=None, xoffset=0, yoffset=-0.5, fontsize='large', horizontalalignment='left', opts={}):
+    def plot_point_site(self, ax, dataset, xkey='longitude', ykey='latitude', site_key='site', transform=None, xoffset=0, yoffset=-0.5, fontsize='large', horizontalalignment='left', opts={}):
         """
         Plot the site information for the given dataset on the map
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
         :param ax: The axis object
         :type ax: matplotlib.axes.Axes
         :param dataset: The dataset to plot
         :type dataset: XCSV object
         :param xkey: The header item key for the coordinate in the x-direction
         :type xkey: str
         :param ykey: The header item key for the coordinate in the y-direction
@@ -260,20 +258,18 @@
             lat = [float(dataset.get_metadata_item_value(ykey))]
 
             ax.plot(lon, lat, transform=transform, color=color, marker=marker)
             ax.text(lon[0] + xoffset, lat[0] + yoffset, site, color=color, fontsize=fontsize, horizontalalignment=horizontalalignment, transform=transform)
         except KeyError:
             pass
 
-    def plot_bbox_site(self, fig, ax, dataset, xminkey='geospatial_lon_min', xmaxkey='geospatial_lon_max', yminkey='geospatial_lat_min', ymaxkey='geospatial_lat_max', site_key='site', transform=None, xoffset=0, yoffset=-0.5, fontsize='large', horizontalalignment='left', opts={}):
+    def plot_bbox_site(self, ax, dataset, xminkey='geospatial_lon_min', xmaxkey='geospatial_lon_max', yminkey='geospatial_lat_min', ymaxkey='geospatial_lat_max', site_key='site', transform=None, xoffset=0, yoffset=-0.5, fontsize='large', horizontalalignment='left', opts={}):
         """
         Plot the site information for the given dataset on the map
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
         :param ax: The axis object
         :type ax: matplotlib.axes.Axes
         :param dataset: The dataset to plot
         :type dataset: XCSV object
         :param xminkey: The header item key for the minimum coordinate in
         the x-direction
         :type xminkey: str
@@ -320,20 +316,18 @@
 
             geom = geometry.box(minx=lon_min, maxx=lon_max, miny=lat_min, maxy=lat_max)
             ax.add_geometries([geom], crs=transform, facecolor=color, edgecolor='black', alpha=alpha)
             ax.text(lon_min + xoffset, lat_min + yoffset, site, color=color, fontsize=fontsize, horizontalalignment=horizontalalignment, transform=transform)
         except KeyError:
             pass
 
-    def plot_site(self, fig, ax, dataset, point_test_key='longitude', bbox_test_key='geospatial_lon_min', site_key='site', transform=None, xoffset=0, yoffset=-0.5, fontsize='large', horizontalalignment='left', opts={}):
+    def plot_site(self, ax, dataset, point_test_key='longitude', bbox_test_key='geospatial_lon_min', site_key='site', transform=None, xoffset=0, yoffset=-0.5, fontsize='large', horizontalalignment='left', opts={}):
         """
         Plot the site information for the given dataset on the map
 
-        :param fig: The figure object
-        :type fig: matplotlib.figure.Figure
         :param ax: The axis object
         :type ax: matplotlib.axes.Axes
         :param dataset: The dataset to plot
         :type dataset: XCSV object
         :param point_test_key: The header item key to test whether coordinates
         are given as a point
         :type point_test_key: str
@@ -357,53 +351,156 @@
         :param opts: Option kwargs to apply to all plots (e.g., color, marker)
         :type opts: dict
         """
 
         # Plot according to whether site coordinates are given by a point
         # or a bounding box
         if point_test_key in dataset.metadata['header']:
-            self.plot_point_site(fig, ax, dataset, site_key=site_key, transform=transform, xoffset=xoffset, yoffset=yoffset, fontsize=fontsize, horizontalalignment=horizontalalignment, opts=opts)
+            self.plot_point_site(ax, dataset, site_key=site_key, transform=transform, xoffset=xoffset, yoffset=yoffset, fontsize=fontsize, horizontalalignment=horizontalalignment, opts=opts)
         elif bbox_test_key in dataset.metadata['header']:
-            self.plot_bbox_site(fig, ax, dataset, site_key=site_key, transform=transform, xoffset=xoffset, yoffset=yoffset, fontsize=fontsize, horizontalalignment=horizontalalignment, opts=opts)
+            self.plot_bbox_site(ax, dataset, site_key=site_key, transform=transform, xoffset=xoffset, yoffset=yoffset, fontsize=fontsize, horizontalalignment=horizontalalignment, opts=opts)
         else:
             raise KeyError(f"Cannot plot site on the map as no spatial coordinate keys were found in the header")
 
-    def setup_figure_and_axes(self, figsize=None, width_ratios=[1,1], projection=None):
+    def setup_figure_and_axes(self, figsize=None, nrows=1, ncols=2, width_ratios=[1,1], projection=None):
         """
         Setup the figure and axes array
 
         If not called directly, then it is called by the plot_datasets()
         function.  If a specific figure size is required, then this function
         should be called directly, before calling any of the plotting
         functions (e.g., plot_datasets()).
 
         This stores the figure object in self.fig and the axes array in
         self.axs.
 
         :param figsize: The figure size tuple as (width, height)
         :type figsize: tuple
-        :param width_ratios: The width ratios of the two subplots - the data
-        plot and the map, in that order.  For example, [2,1] will make the
-        plot twice the size of the map
+        :param nrows: The number of rows for the subplots (1 or 2)
+        :type nrows: int
+        :param ncols: The number of columns for the subplots (1 or 2)
+        :type ncols: int
+        :param width_ratios: The width ratios of the subplots.  If there is
+        only one subplot, then it is the map, and this should be [1].  If
+        there are two subplots, then these are the data plot and the map, in
+        that order.  For example, [2,1] will make the plot twice the size of
+        the map
         :type width_ratios: list
         :param projection: The projection to transform the coordinates on the
         map.  If not specified, it defaults to ccrs.PlateCarree()
         :type projection: cartopy.crs.CRS
         """
 
         if not projection:
             projection = ccrs.PlateCarree()
 
         self.fig = plt.figure(figsize=figsize)
-        gs = self.fig.add_gridspec(1, 2, width_ratios=width_ratios)
+        gs = self.fig.add_gridspec(nrows=nrows, ncols=ncols, width_ratios=width_ratios)
+
+        if nrows * ncols > 1:
+            self.axs.append(self.fig.add_subplot(gs[0, 0]))
+            self.axs.append(self.fig.add_subplot(gs[0, 1], projection=projection))
+        else:
+            self.axs.append(self.fig.add_subplot(gs[0, 0], projection=projection))
+
+    def _setup_fallback_figure_and_axes(self, fig=None, axs=None, plot_on_map=False):
+        """
+        Setup a fallback figure and axes array
+
+        This calls setup_figure_and_axes() if it hasn't already beeen called
+
+        :param fig: The figure object
+        :type fig: matplotlib.figure.Figure
+        :param axs: The axes array
+        :type axs: matplotlib.axes.Axes
+        :param plot_on_map: Only setup a map, as the data are to be plotted
+        directly on the map
+        :type plot_on_map: bool
+        """
+
+        if fig:
+            self.fig = fig
+
+        if axs:
+            self.axs = axs
+
+        if not self.fig or not self.axs:
+            fa_opts = {'nrows': 1, 'ncols': 2, 'width_ratios': [1,1]}
+
+            if plot_on_map:
+                fa_opts = {'nrows': 1, 'ncols': 1, 'width_ratios': [1]}
+
+            self.setup_figure_and_axes(**fa_opts)
+
+    def _add_figure_annotations(self, axs_idx=0, map_axs_idx=1, plot_on_map=False):
+        """
+        Add annotations to the figure
+
+        :param axs_idx: The index of the axis object in the axs array
+        :type axs_idx: int
+        :param map_axs_idx: The index of the map axis object in the axs array
+        :type map_axs_idx: int
+        :param plot_on_map: Only setup a map, as the data are to be plotted
+        directly on the map
+        :type plot_on_map: bool
+        """
+
+        self.add_figure_title(self.title)
+        self.add_figure_caption(self.caption)
+
+        if plot_on_map:
+            self.setup_site_plot(self.axs[axs_idx], self.get_site_plot_extent(self.datasets))
+        else:
+            self.setup_data_plot(self.axs[axs_idx], xlabel=self.xlabel, ylabel=self.ylabel)
+            self.setup_site_plot(self.axs[map_axs_idx], self.get_site_plot_extent(self.datasets))
+
+    def _plot_datasets(self, axs_idx=0, map_axs_idx=1, plot_on_map=False, invert_xaxis=False, invert_yaxis=False, opts={}):
+        """
+        Plot the data for the figure datasets
+
+        :param axs_idx: The index of the axis object in the axs array
+        :type axs_idx: int
+        :param map_axs_idx: The index of the map axis object in the axs array
+        :type map_axs_idx: int
+        :param plot_on_map: Only setup a map, as the data are to be plotted
+        directly on the map
+        :type plot_on_map: bool
+        :param invert_xaxis: Invert the x-axis
+        :type invert_xaxis: bool
+        :param invert_yaxis: Invert the y-axis
+        :type invert_yaxis: bool
+        :param opts: Option kwargs to apply to all plots (e.g., color, marker)
+        :type opts: dict
+        """
+
+        generate_colors = True
+
+        if 'color' in opts:
+            generate_colors = False
+
+        for i, dataset in enumerate(self.datasets):
+            label = dataset.get_metadata_item_value(self.label_key)
+
+            if generate_colors:
+                opts.update({'color': f'C{i}'})
 
-        self.axs.append(self.fig.add_subplot(gs[0, 0]))
-        self.axs.append(self.fig.add_subplot(gs[0, 1], projection=projection))
+            if plot_on_map:
+                projection = self.axs[axs_idx].projection
 
-    def plot_datasets(self, datasets, fig=None, axs=None, axs_idx=0, map_axs_idx=1, xcol=None, ycol=None, xidx=None, yidx=0, xlabel=None, ylabel=None, title=None, title_wrap=True, caption=None, label_key=None, invert_xaxis=False, invert_yaxis=False, show=True, opts={}):
+                if not projection:
+                    projection = ccrs.PlateCarree()
+
+                opts.update({'transform': projection})
+
+                self.plot_data(self.axs[axs_idx], dataset, self.xcol, self.ycol, label=label, invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis, opts=opts)
+            else:
+                self.plot_data(self.axs[axs_idx], dataset, self.xcol, self.ycol, label=label, invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis, opts=opts)
+                self.plot_site(self.axs[map_axs_idx], dataset, site_key=self.label_key, opts=opts)
+
+    def plot_datasets(self, datasets, fig=None, axs=None, axs_idx=0, map_axs_idx=1, xcol=None, ycol=None, xidx=None, yidx=0, xlabel=None, ylabel=None, title=None, caption=None, label_key=None, invert_xaxis=False, invert_yaxis=False, plot_on_map=False, show=True, opts={}):
         """
         Plot the data for the given datasets
 
         Either the xcol and ycol column header labels, or the xidx and yidx
         column indices, can be specified.  These are mutually exclusive.  They
         identify the data series from the datasets' data tables to be used for
         the x- and y-axis data.
@@ -438,79 +535,34 @@
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
         :param invert_xaxis: Invert the x-axis
         :type invert_xaxis: bool
         :param invert_yaxis: Invert the y-axis
         :type invert_yaxis: bool
+        :param plot_on_map: Instead of plotting the data on a plot alongside
+        the site map, show just a map and plot the data directly on the map.
+        This requires the data to be coordinates
+        :type plot_on_map: bool
         :param show: Show the plot
         :type show: bool
         :param opts: Option kwargs to apply to all plots (e.g., color, marker)
         :type opts: dict
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
-
-        self.datasets = datasets
-        self.xcol = xcol
-        self.ycol = ycol
-        generate_colors = True
-
-        if not title:
-            title = datasets[0].get_metadata_item_value(self.DEFAULTS['title_key'])
-
-        if not caption:
-            caption = datasets[0].get_metadata_item_value(self.DEFAULTS['caption_key'])
-
-        if not label_key:
-            label_key = self.DEFAULTS['label_key']
-
-        if not xcol:
-            if xidx is not None:
-                self.xcol = datasets[0].data.iloc[:, xidx].name
-
-        if not ycol:
-            self.ycol = datasets[0].data.iloc[:, yidx].name
-
-        if not xlabel:
-            xlabel = self.xcol
-
-        if not ylabel:
-            ylabel = self.ycol
-
-        if 'color' in opts:
-            generate_colors = False
-
-        self.fig.suptitle(title, wrap=title_wrap)
-        self.setup_data_plot(self.fig, self.axs[axs_idx], caption=caption, xlabel=xlabel, ylabel=ylabel)
-        self.setup_site_plot(self.fig, self.axs[map_axs_idx], self.get_site_plot_extent(datasets))
-
-        for i, dataset in enumerate(datasets):
-            label = dataset.get_metadata_item_value(label_key)
-
-            if generate_colors:
-                opts.update({'color': f'C{i}'})
 
-            self.plot_data(self.fig, self.axs[axs_idx], dataset, self.xcol, self.ycol, label=label, invert_xaxis=invert_xaxis, invert_yaxis=invert_yaxis, opts=opts)
-            self.plot_site(self.fig, self.axs[map_axs_idx], dataset, site_key=label_key, opts=opts)
+        self._setup_fallback_figure_and_axes(fig, axs, plot_on_map)
+        self._store_figure_parameters(datasets, xcol, ycol, xidx, yidx, xlabel, ylabel, title, caption, label_key)
+        self._add_figure_annotations(axs_idx, map_axs_idx, plot_on_map)
+        self._plot_datasets(axs_idx, map_axs_idx, plot_on_map, invert_xaxis, invert_yaxis, opts)
 
         if show:
             plt.show()
```

### Comparing `xcsv_plot_map-0.3.0/xcsv/plot_map/__main__.py` & `xcsv_plot_map-0.4.0/xcsv/plot_map/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,16 @@
     parser.add_argument('--title', help='text to be used for the plot title', dest='title', default=None, type=str)
     parser.add_argument('--caption', help='text to be used for the plot caption', dest='caption', default=None, type=str)
     parser.add_argument('--label-key', help='key of the header item in the extended header section whose value will be used for the plot legend label', dest='label_key', default=None, type=str)
 
     parser.add_argument('-s', '--figsize', help='size of the figure (width height)', dest='figsize', nargs=2, default=None, type=int)
     parser.add_argument('-p', '--map-projection', help='projection to use for displaying the site coordinates on the map (one of the CRS classes provided by Cartopy)', dest='projection', default=None, type=str)
 
+    parser.add_argument('-m', '--plot-on-map', help='instead of a plot alongside a site map, show just a map and plot the coordinate data directly on the map', dest='plot_on_map', action='store_true', default=False)
+
     parser.add_argument('-b', '--background-image', help='path to an image to show in the background of the plot', dest='bg_img_path', default=None, type=str)
 
     parser.add_argument('-o', '--out-file', help='output plot file')
 
     parser.add_argument('-P', '--plot-options', help="options for the plot, specified as a simple JSON object", dest='plot_opts', default={}, type=json.loads)
     parser.add_argument('-S', '--scatter-plot', help="set plot options (see -P) to produce a scatter plot", dest='plot_opts', action='store_const', const={'marker': '.', 'ls': ''})
 
@@ -115,23 +117,26 @@
     Main function
     """
 
     args = parse_cmdln()
     datasets = get_datasets(args.in_file)
     plotter = xpm.Plot()
 
-    if args.figsize or args.projection:
+    if args.figsize or args.projection or args.plot_on_map:
+        fa_opts = {'figsize': args.figsize}
+
         if args.projection:
-            projection = xpm.Plot().get_crs_class_from_string(args.projection)
-        else:
-            projection = None
+            fa_opts['projection'] = xpm.Plot().get_crs_class_from_string(args.projection)
+
+        if args.plot_on_map:
+            fa_opts.update({'nrows': 1, 'ncols': 1, 'width_ratios': [1]})
 
-        plotter.setup_figure_and_axes(figsize=args.figsize, projection=projection)
+        plotter.setup_figure_and_axes(**fa_opts)
 
-    plotter.plot_datasets(datasets, xidx=args.xidx, yidx=args.yidx, xcol=args.xcol, ycol=args.ycol, xlabel=args.xlabel, ylabel=args.ylabel, title=args.title, title_wrap=True, caption=args.caption, label_key=args.label_key, invert_xaxis=args.invert_xaxis, invert_yaxis=args.invert_yaxis, show=False, opts=args.plot_opts)
+    plotter.plot_datasets(datasets, xidx=args.xidx, yidx=args.yidx, xcol=args.xcol, ycol=args.ycol, xlabel=args.xlabel, ylabel=args.ylabel, title=args.title, caption=args.caption, label_key=args.label_key, invert_xaxis=args.invert_xaxis, invert_yaxis=args.invert_yaxis, plot_on_map=args.plot_on_map, show=False, opts=args.plot_opts)
 
     if args.bg_img_path:
         plotter.add_plot_bg(img_path=args.bg_img_path)
 
     if args.out_file:
         plotter.savefig(args.out_file)
     else:
```

### Comparing `xcsv_plot_map-0.3.0/setup.py` & `xcsv_plot_map-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 {'': ['*']}
 
 install_requires = \
 ['Cartopy>=0.21.1,<0.22.0',
  'matplotlib>=3.5.2,<4.0.0',
  'scipy>=1.8.1,<2.0.0',
  'shapely>=2.0.1,<3.0.0',
- 'xcsv-plot>=0.3.0,<0.4.0']
+ 'xcsv-plot>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['xcsv_plot_map = xcsv.plot_map.__main__:main']}
 
 setup_kwargs = {
     'name': 'xcsv-plot-map',
-    'version': '0.3.0',
+    'version': '0.4.0',
     'description': 'Subpackage to plot and locate on a map, data from extended CSV (XCSV) files',
-    'long_description': "# xcsv-plot-map\n\nxcsv-plot-map is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files, and locating the data on a map, given an extended header section with geographical coordinates.  These will typically detail where the data were acquired.  It inherits from the [xcsv-plot](https://pypi.org/project/xcsv-plot) subpackage of xcsv.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv-plot-map\n```\n\n## Notes on installing Cartopy\n\nxcsv-plot-map has a dependency on Cartopy.  In turn, Cartopy requires the Proj library.  If you find that you can't install Cartopy because the version of the Proj library on your system is too old, then you can build a local version of the Proj library.  This should be a fairly straightforward build.  You may then find that the Cartopy package installs OK, but that you get the following segfault at runtime when trying to use xcsv-plot-map:\n\n```bash\nfree(): invalid size\nAborted (core dumped)\n```\n\nThis is a known issue.  A suggested fix for this is to reinstall the Python `shapely` package.  First remove it:\n\n```bash\n$ pip uninstall shapely\n```\n\nand then reinstall it with specific `pip` options:\n\n```bash\n$ pip install --no-binary :all: shapely\n```\n\nThis may take a while, but should resolve the segfault issue and everything should work.\n\n## Using the package\n\nAn XCSV file with an [ACDD-compliant](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3) extended header section, including geographical coordinates in `longitude` and `latitude` header items, and well-annotated column-headers, already provides much of the text needed to make an informative plot and map, so we can just plot the XCSV file directly from the command line.  This is the purpose of the `xcsv-plot-map` subpackage.  For example:\n\n```bash\n$ python3 -m xcsv.plot_map -x 0 -y 1 example.csv\n```\n\nNote here that we're calling `xcsv-plot-map` as a *module main*.  As a convenience, this invocation is wrapped as a console script when installing the package, hence the following invocation is equivalent:\n\n```bash\n$ xcsv_plot_map -x 0 -y 1 example.csv\n```\n\nIn addition to using the CLI, the package can be used as a Python library.  The main class is `Plot`.  This is inherited from the `xcsv-plot.Plot` class, with some overridden methods.  The class provides methods to plot a given list of datasets (XCSV objects), and locate them on a map:\n\n```python\nimport xcsv\nimport xcsv.plot_map as xpm\n\nfilenames = ['example1.csv','example2.csv','example3.csv']\ndatasets = []\n\nfor filename in filenames:\n    with xcsv.File(filename) as f:\n        datasets.append(f.read())\n\nplotter = xpm.Plot()\nplotter.plot_datasets(datasets, xidx=0, yidx=1)\n```\n\n## Command line usage\n\nCalling the script with the `--help` option will show the following usage:\n\n```bash\n$ python -m xcsv.plot_map --help\nusage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]\n                     [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]\n                     [--invert-y-axis] [--title TITLE] [--caption CAPTION]\n                     [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]\n                     [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]\n                     [-P PLOT_OPTS] [-S] [-V]\n                     in_file [in_file ...]\n\nplot the given XCSV files and locate the data on a map\n\npositional arguments:\n  in_file               input XCSV file(s)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -x XIDX, --x-idx XIDX\n                        column index (zero-based) containing values for the\n                        x-axis\n  -X XCOL, --x-column XCOL\n                        column label containing values for the x-axis\n  -y YIDX, --y-idx YIDX\n                        column index (zero-based) containing values for the\n                        y-axis\n  -Y YCOL, --y-column YCOL\n                        column label containing values for the y-axis\n  --x-label XLABEL      text to be used for the plot x-axis label\n  --y-label YLABEL      text to be used for the plot y-axis label\n  --invert-x-axis       invert the x-axis\n  --invert-y-axis       invert the y-axis\n  --title TITLE         text to be used for the plot title\n  --caption CAPTION     text to be used for the plot caption\n  --label-key LABEL_KEY\n                        key of the header item in the extended header section\n                        whose value will be used for the plot legend label\n  -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE\n                        size of the figure (width height)\n  -p PROJECTION, --map-projection PROJECTION\n                        projection to use for displaying the site coordinates\n                        on the map (one of the CRS classes provided by\n                        Cartopy)\n  -b BG_IMG_PATH, --background-image BG_IMG_PATH\n                        path to an image to show in the background of the plot\n  -o OUT_FILE, --out-file OUT_FILE\n                        output plot file\n  -P PLOT_OPTS, --plot-options PLOT_OPTS\n                        options for the plot, specified as a simple JSON\n                        object\n  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot\n  -V, --version         show program's version number and exit\n\nExamples\n\nGiven an XCSV file with an ACDD-compliant extended header section, including geographical coordinates in longitude and latitude, and a single column (at column 0) of data values:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ndepth (m)\n0.575\n1.125\n2.225\n\nThen the following invocation will plot the only column on the y-axis, with the x-axis the indices of the data points, and will locate the coordinates on a map:\n\npython3 -m xcsv.plot_map input.csv\n\nIf the file also contains a suitable variable for the x-axis:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n\nthen the columns to be used for the x- and y-axes can be specified thus:\n\npython3 -m xcsv.plot_map -x 0 -y 1 input.csv\n```\n\n",
+    'long_description': "# xcsv-plot-map\n\nxcsv-plot-map is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files, and locating the data on a map, given an extended header section with geographical coordinates.  These will typically detail where the data were acquired.  It inherits from the [xcsv-plot](https://pypi.org/project/xcsv-plot) subpackage of xcsv.\n\n## Install\n\nThe package can be installed from PyPI:\n\n```bash\n$ pip install xcsv-plot-map\n```\n\n## Notes on installing Cartopy\n\nxcsv-plot-map has a dependency on Cartopy.  In turn, Cartopy requires the Proj library.  If you find that you can't install Cartopy because the version of the Proj library on your system is too old, then you can build a local version of the Proj library.  This should be a fairly straightforward build.  You may then find that the Cartopy package installs OK, but that you get the following segfault at runtime when trying to use xcsv-plot-map:\n\n```bash\nfree(): invalid size\nAborted (core dumped)\n```\n\nThis is a known issue.  A suggested fix for this is to reinstall the Python `shapely` package.  First remove it:\n\n```bash\n$ pip uninstall shapely\n```\n\nand then reinstall it with specific `pip` options:\n\n```bash\n$ pip install --no-binary :all: shapely\n```\n\nThis may take a while, but should resolve the segfault issue and everything should work.\n\n## Using the package\n\nAn XCSV file with an [ACDD-compliant](https://wiki.esipfed.org/Attribute_Convention_for_Data_Discovery_1-3) extended header section, including geographical coordinates in `longitude` and `latitude` header items, and well-annotated column-headers, already provides much of the text needed to make an informative plot and map, so we can just plot the XCSV file directly from the command line.  This is the purpose of the `xcsv-plot-map` subpackage.  For example:\n\n```bash\n$ python3 -m xcsv.plot_map -x 0 -y 1 example.csv\n```\n\nNote here that we're calling `xcsv-plot-map` as a *module main*.  As a convenience, this invocation is wrapped as a console script when installing the package, hence the following invocation is equivalent:\n\n```bash\n$ xcsv_plot_map -x 0 -y 1 example.csv\n```\n\nIn addition to using the CLI, the package can be used as a Python library.  The main class is `Plot`.  This is inherited from the `xcsv-plot.Plot` class, with some overridden methods.  The class provides methods to plot a given list of datasets (XCSV objects), and locate them on a map:\n\n```python\nimport xcsv\nimport xcsv.plot_map as xpm\n\nfilenames = ['example1.csv','example2.csv','example3.csv']\ndatasets = []\n\nfor filename in filenames:\n    with xcsv.File(filename) as f:\n        datasets.append(f.read())\n\nplotter = xpm.Plot()\nplotter.plot_datasets(datasets, xidx=0, yidx=1)\n```\n\n## Command line usage\n\nCalling the script with the `--help` option will show the following usage:\n\n```bash\n$ python -m xcsv.plot_map --help\nusage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]\n                     [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]\n                     [--invert-y-axis] [--title TITLE] [--caption CAPTION]\n                     [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]\n                     [-p PROJECTION] [-m] [-b BG_IMG_PATH] [-o OUT_FILE]\n                     [-P PLOT_OPTS] [-S] [-V]\n                     in_file [in_file ...]\n\nplot the given XCSV files and locate the data on a map\n\npositional arguments:\n  in_file               input XCSV file(s)\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -x XIDX, --x-idx XIDX\n                        column index (zero-based) containing values for the\n                        x-axis\n  -X XCOL, --x-column XCOL\n                        column label containing values for the x-axis\n  -y YIDX, --y-idx YIDX\n                        column index (zero-based) containing values for the\n                        y-axis\n  -Y YCOL, --y-column YCOL\n                        column label containing values for the y-axis\n  --x-label XLABEL      text to be used for the plot x-axis label\n  --y-label YLABEL      text to be used for the plot y-axis label\n  --invert-x-axis       invert the x-axis\n  --invert-y-axis       invert the y-axis\n  --title TITLE         text to be used for the plot title\n  --caption CAPTION     text to be used for the plot caption\n  --label-key LABEL_KEY\n                        key of the header item in the extended header section\n                        whose value will be used for the plot legend label\n  -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE\n                        size of the figure (width height)\n  -p PROJECTION, --map-projection PROJECTION\n                        projection to use for displaying the site coordinates\n                        on the map (one of the CRS classes provided by\n                        Cartopy)\n  -m, --plot-on-map     instead of a plot alongside a site map, show just a\n                        map and plot the coordinate data directly on the map\n  -b BG_IMG_PATH, --background-image BG_IMG_PATH\n                        path to an image to show in the background of the plot\n  -o OUT_FILE, --out-file OUT_FILE\n                        output plot file\n  -P PLOT_OPTS, --plot-options PLOT_OPTS\n                        options for the plot, specified as a simple JSON\n                        object\n  -S, --scatter-plot    set plot options (see -P) to produce a scatter plot\n  -V, --version         show program's version number and exit\n\nExamples\n\nGiven an XCSV file with an ACDD-compliant extended header section, including geographical coordinates in longitude and latitude, and a single column (at column 0) of data values:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ndepth (m)\n0.575\n1.125\n2.225\n\nThen the following invocation will plot the only column on the y-axis, with the x-axis the indices of the data points, and will locate the coordinates on a map:\n\npython3 -m xcsv.plot_map input.csv\n\nIf the file also contains a suitable variable for the x-axis:\n\n# id: 1\n# title: The title\n# latitude: -73.86 (degree_north)\n# longitude: -65.46 (degree_east)\ntime (year) [a],depth (m)\n2012,0.575\n2011,1.125\n2010,2.225\n\nthen the columns to be used for the x- and y-axes can be specified thus:\n\npython3 -m xcsv.plot_map -x 0 -y 1 input.csv\n```\n\n",
     'author': 'Paul Breen',
     'author_email': 'pbree@bas.ac.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/paul-breen/xcsv-plot-map',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `xcsv_plot_map-0.3.0/PKG-INFO` & `xcsv_plot_map-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcsv-plot-map
-Version: 0.3.0
+Version: 0.4.0
 Summary: Subpackage to plot and locate on a map, data from extended CSV (XCSV) files
 Home-page: https://github.com/paul-breen/xcsv-plot-map
 License: Apache-2.0
 Author: Paul Breen
 Author-email: pbree@bas.ac.uk
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Cartopy (>=0.21.1,<0.22.0)
 Requires-Dist: matplotlib (>=3.5.2,<4.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
-Requires-Dist: xcsv-plot (>=0.3.0,<0.4.0)
+Requires-Dist: xcsv-plot (>=0.4.0,<0.5.0)
 Project-URL: Documentation, https://github.com/paul-breen/xcsv-plot-map/blob/main/README.md
 Project-URL: Repository, https://github.com/paul-breen/xcsv-plot-map
 Description-Content-Type: text/markdown
 
 # xcsv-plot-map
 
 xcsv-plot-map is a subpackage of [xcsv](https://github.com/paul-breen/xcsv).  It's main purpose is to provide a simple CLI for plotting extended CSV (XCSV) files, and locating the data on a map, given an extended header section with geographical coordinates.  These will typically detail where the data were acquired.  It inherits from the [xcsv-plot](https://pypi.org/project/xcsv-plot) subpackage of xcsv.
@@ -93,15 +93,15 @@
 
 ```bash
 $ python -m xcsv.plot_map --help
 usage: xcsv_plot_map [-h] [-x XIDX | -X XCOL] [-y YIDX | -Y YCOL]
                      [--x-label XLABEL] [--y-label YLABEL] [--invert-x-axis]
                      [--invert-y-axis] [--title TITLE] [--caption CAPTION]
                      [--label-key LABEL_KEY] [-s FIGSIZE FIGSIZE]
-                     [-p PROJECTION] [-b BG_IMG_PATH] [-o OUT_FILE]
+                     [-p PROJECTION] [-m] [-b BG_IMG_PATH] [-o OUT_FILE]
                      [-P PLOT_OPTS] [-S] [-V]
                      in_file [in_file ...]
 
 plot the given XCSV files and locate the data on a map
 
 positional arguments:
   in_file               input XCSV file(s)
@@ -129,14 +129,16 @@
                         whose value will be used for the plot legend label
   -s FIGSIZE FIGSIZE, --figsize FIGSIZE FIGSIZE
                         size of the figure (width height)
   -p PROJECTION, --map-projection PROJECTION
                         projection to use for displaying the site coordinates
                         on the map (one of the CRS classes provided by
                         Cartopy)
+  -m, --plot-on-map     instead of a plot alongside a site map, show just a
+                        map and plot the coordinate data directly on the map
   -b BG_IMG_PATH, --background-image BG_IMG_PATH
                         path to an image to show in the background of the plot
   -o OUT_FILE, --out-file OUT_FILE
                         output plot file
   -P PLOT_OPTS, --plot-options PLOT_OPTS
                         options for the plot, specified as a simple JSON
                         object
```

