# Comparing `tmp/p3lib-1.1.8.tar.gz` & `tmp/p3lib-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/scratch/git_repos/python3/p3lib/dist/tmpy2jg2w6g/p3lib-1.1.8.tar", last modified: Wed May 26 19:17:03 2021, max compression
+gzip compressed data, was "/scratch/git_repos/python3/p3lib/dist/tmptcawi2vi/p3lib-1.1.9.tar", last modified: Fri May 28 08:38:41 2021, max compression
```

## Comparing `p3lib-1.1.8.tar` & `p3lib-1.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-26 19:17:03.797519 p3lib-1.1.8/
--rw-rw-r--   0 pja       (1000) pja       (1000)     1067 2021-05-07 19:30:55.000000 p3lib-1.1.8/LICENSE
--rw-rw-r--   0 pja       (1000) pja       (1000)      894 2021-05-26 19:17:03.797519 p3lib-1.1.8/PKG-INFO
--rw-rw-r--   0 pja       (1000) pja       (1000)      274 2021-05-07 19:30:55.000000 p3lib-1.1.8/README.md
--rw-rw-r--   0 pja       (1000) pja       (1000)      103 2021-05-07 19:30:55.000000 p3lib-1.1.8/pyproject.toml
--rw-rw-r--   0 pja       (1000) pja       (1000)      708 2021-05-26 19:17:03.797519 p3lib-1.1.8/setup.cfg
-drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-26 19:17:03.797519 p3lib-1.1.8/src/
-drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-26 19:17:03.797519 p3lib-1.1.8/src/p3lib/
--rw-rw-r--   0 pja       (1000) pja       (1000)        0 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/__init__.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    15623 2021-05-26 19:07:16.000000 p3lib-1.1.8/src/p3lib/bokeh_gui.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    10270 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/boot_manager.py
--rw-rw-r--   0 pja       (1000) pja       (1000)     9429 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/database_if.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    11862 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/helper.py
--rw-rw-r--   0 pja       (1000) pja       (1000)     6973 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/json_networking.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    10511 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/mqtt_rpc.py
--rw-rw-r--   0 pja       (1000) pja       (1000)     9275 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/netif.py
--rw-rw-r--   0 pja       (1000) pja       (1000)     9363 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/netplotly.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    29433 2021-05-26 05:37:01.000000 p3lib-1.1.8/src/p3lib/pconfig.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    32988 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/ssh.py
--rw-rw-r--   0 pja       (1000) pja       (1000)    12876 2021-05-07 19:30:55.000000 p3lib-1.1.8/src/p3lib/uio.py
-drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-26 19:17:03.797519 p3lib-1.1.8/src/p3lib.egg-info/
--rw-rw-r--   0 pja       (1000) pja       (1000)      894 2021-05-26 19:17:03.000000 p3lib-1.1.8/src/p3lib.egg-info/PKG-INFO
--rw-rw-r--   0 pja       (1000) pja       (1000)      438 2021-05-26 19:17:03.000000 p3lib-1.1.8/src/p3lib.egg-info/SOURCES.txt
--rw-rw-r--   0 pja       (1000) pja       (1000)        1 2021-05-26 19:17:03.000000 p3lib-1.1.8/src/p3lib.egg-info/dependency_links.txt
--rw-rw-r--   0 pja       (1000) pja       (1000)        6 2021-05-26 19:17:03.000000 p3lib-1.1.8/src/p3lib.egg-info/top_level.txt
+drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-28 08:38:41.868298 p3lib-1.1.9/
+-rw-rw-r--   0 pja       (1000) pja       (1000)     1067 2021-05-07 19:30:55.000000 p3lib-1.1.9/LICENSE
+-rw-rw-r--   0 pja       (1000) pja       (1000)      894 2021-05-28 08:38:41.868298 p3lib-1.1.9/PKG-INFO
+-rw-rw-r--   0 pja       (1000) pja       (1000)      274 2021-05-07 19:30:55.000000 p3lib-1.1.9/README.md
+-rw-rw-r--   0 pja       (1000) pja       (1000)      103 2021-05-07 19:30:55.000000 p3lib-1.1.9/pyproject.toml
+-rw-rw-r--   0 pja       (1000) pja       (1000)      708 2021-05-28 08:38:41.872298 p3lib-1.1.9/setup.cfg
+drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-28 08:38:41.868298 p3lib-1.1.9/src/
+drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-28 08:38:41.868298 p3lib-1.1.9/src/p3lib/
+-rw-rw-r--   0 pja       (1000) pja       (1000)        0 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/__init__.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    15588 2021-05-28 08:31:06.000000 p3lib-1.1.9/src/p3lib/bokeh_gui.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    10270 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/boot_manager.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)     9429 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/database_if.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    11862 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/helper.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)     6973 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/json_networking.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    10511 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/mqtt_rpc.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)     9275 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/netif.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)     9363 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/netplotly.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    29433 2021-05-26 05:37:01.000000 p3lib-1.1.9/src/p3lib/pconfig.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    32988 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/ssh.py
+-rw-rw-r--   0 pja       (1000) pja       (1000)    12876 2021-05-07 19:30:55.000000 p3lib-1.1.9/src/p3lib/uio.py
+drwxrwxr-x   0 pja       (1000) pja       (1000)        0 2021-05-28 08:38:41.868298 p3lib-1.1.9/src/p3lib.egg-info/
+-rw-rw-r--   0 pja       (1000) pja       (1000)      894 2021-05-28 08:38:41.000000 p3lib-1.1.9/src/p3lib.egg-info/PKG-INFO
+-rw-rw-r--   0 pja       (1000) pja       (1000)      438 2021-05-28 08:38:41.000000 p3lib-1.1.9/src/p3lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 pja       (1000) pja       (1000)        1 2021-05-28 08:38:41.000000 p3lib-1.1.9/src/p3lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 pja       (1000) pja       (1000)        6 2021-05-28 08:38:41.000000 p3lib-1.1.9/src/p3lib.egg-info/top_level.txt
```

### Comparing `p3lib-1.1.8/LICENSE` & `p3lib-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/PKG-INFO` & `p3lib-1.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3lib
-Version: 1.1.8
+Version: 1.1.9
 Summary: A group of python modules for networking, plotting data, config storage, automating boot scripts, ssh access and user input output.
 Home-page: https://github.com/pjaos/p3lib
 Author: Paul Austen
 Author-email: pausten.os@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pjaos/p3lib/issues
 Platform: UNKNOWN
```

### Comparing `p3lib-1.1.8/setup.cfg` & `p3lib-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = p3lib
-version = 1.1.8
+version = 1.1.9
 author = Paul Austen
 author_email = pausten.os@gmail.com
 description = A group of python modules for networking, plotting data, config storage, automating boot scripts, ssh access and user input output.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/pjaos/p3lib
 project_urls =
```

### Comparing `p3lib-1.1.8/src/p3lib/bokeh_gui.py` & `p3lib-1.1.9/src/p3lib/bokeh_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                      x_axis_location="below",
                      y_range=yrange,
                      plot_width=width,
                      plot_height=height)
         fig.yaxis.axis_label = yAxisName
         return fig
 
-    
+
     def __init__(self, docTitle, topCtrlPanel=True, bokehPort=9090):
         """@brief Constructor.
            @param docTitle The document title.
            @param topCtrlPanel If True then a control panel is displayed at the top of the plot.
            @param bokehPort The port to run the server on."""
         self._docTitle=docTitle
         self._topCtrlPanel=topCtrlPanel
@@ -146,24 +146,30 @@
     def runBokehServer(self):
         """@brief Run the bokeh server. This is a blocking method."""
         apps = {'/': Application(FunctionHandler(self.createPlot))}
         self._server = Server(apps, port=9000)
         self._server.show("/")
         self._server.run_until_shutdown()
 
-                
+
 class TimeSeriesPlotter(TabbedGUI):
     """@brief Responsible for plotting data on tab 0 with no other tabs."""
 
-    def __init__(self, docTitle, bokehPort=5001):
-        """@Constructor"""
+    def __init__(self, docTitle, showCtrl=True, bokehPort=5001):
+        """@Constructor
+           @param docTitle  The web page title that will appear in the browser tab.
+           @param showCtrl  Show the control panel at the top of the plot. Only
+                            really useful if the plot is real time.
+           @param bokehPort The TCP server port for the bokeh server."""
         super().__init__(docTitle, bokehPort=bokehPort)
         self._statusAreaInput = None
         self._figTable=[[]]
         self._grid = None
+        self._showCtrl = showCtrl
+        self._fileToSave = None
 
     def addRow(self):
         """@brief Add an empty row to the figures."""
         self._figTable.append([])
 
     def addToRow(self, fig):
         """@brief Add a figure to the end of the current row of figues.
@@ -177,182 +183,178 @@
         self._doc.title = self._docTitle
 
         plotPanel = self._getPlotPanel()
 
         self._tabList.append( Panel(child=plotPanel,  title="Plots") )
         self._doc.add_root( Tabs(tabs=self._tabList) )
         self._doc.add_periodic_callback(self._update, 100)
-            
+
     def _getPlotPanel(self):
         """@brief Add tab that shows plot data updates."""
         self._grid = gridplot(children = self._figTable, sizing_mode = 'scale_both',  toolbar_location='left')
 
-        checkbox1 = CheckboxGroup(labels=["Plot Data"], active=[0, 1],max_width=70)
-        checkbox1.on_change('active', self._checkboxHandler)
+        if self._showCtrl:
+            checkbox1 = CheckboxGroup(labels=["Plot Data"], active=[0, 1],max_width=70)
+            checkbox1.on_change('active', self._checkboxHandler)
 
-        self.fileToSave = TextInput(title="File to save", max_width=150)
+            self._fileToSave = TextInput(title="File to save", max_width=150)
 
-        saveButton = Button(label="Save", button_type="success", width=50)
-        saveButton.on_click(self._savePlot)
+            saveButton = Button(label="Save", button_type="success", width=50)
+            saveButton.on_click(self._savePlot)
 
-        shutDownButton = Button(label="Quit", button_type="success", width=50)
-        shutDownButton.on_click(self.stopServer)
+            shutDownButton = Button(label="Quit", button_type="success", width=50)
+            shutDownButton.on_click(self.stopServer)
 
-        self._statusAreaInput = TextAreaInput(value="", width_policy="max")
-        statusPanel = row([self._statusAreaInput])
+            plotRowCtrl = row(children=[checkbox1, saveButton, self._fileToSave, shutDownButton])
+            plotPanel = column([plotRowCtrl, self._grid])
+        else:
+            plotPanel = column([self._grid])
 
-        plotRowCtrl = row(children=[checkbox1, saveButton, self.fileToSave, shutDownButton])
-        plotPanel = column([plotRowCtrl, self._grid, statusPanel])
         return plotPanel
 
     def _savePlot(self):
         """@brief Save plot to a single html file. This allows the plots to be
                   analysed later."""
-        if self.fileToSave.value:
+        if self._fileToSave and self._fileToSave.value:
             if self.fileToSave.value.endswith(".html"):
                 filename = self.fileToSave.value
             else:
                 filename = self.fileToSave.value + ".html"
             output_file(filename)
             # Save all the plots in the grid to an html file that allows
             # display in a browser and plot manipulation.
             save( self._grid )
-            self._statusAreaInput.value = "Saved {}".format(filename)
 
     def _checkboxHandler(self, attr, old, new):
         """@brief Called when the checkbox is clicked."""
         if 0 in list(new):  # Is first checkbox selected
             self._plottingEnabled = True
-            self._statusAreaInput.value = "Plotting enabled"
         else:
             self._plottingEnabled = False
-            self._statusAreaInput.value = "Plotting disabled"
-            
-            
-        
+
+
+
 class StatusBarWrapper(object):
-    """@brief Responsible for presenting a single status line of text in a GUI 
-              that runs the width of the page (normally at the bottom)."""    
+    """@brief Responsible for presenting a single status line of text in a GUI
+              that runs the width of the page (normally at the bottom)."""
     def __init__(self):
         data = dict(
             status = [],
         )
         self.source = ColumnDataSource(data)
-    
+
         columns = [
                 TableColumn(field="status", title="status"),
             ]
         self.statusBar = DataTable(source=self.source, columns=columns, height_policy="fixed", height=50, header_row=False, index_position=None)
-        
+
     def getWidget(self):
         """@brief return an instance of the status bar widget to be added to a layout."""
         return self.statusBar
-    
+
     def setStatus(self, msg):
         """@brief Set the message iun the status bar.
            @param The message to be displayed."""
         self.source.data = {"status": [msg]}
-        
+
 class ReadOnlyTableWrapper(object):
-    """@brief Responsible for presenting a table of values that can be updated dynamically."""    
+    """@brief Responsible for presenting a table of values that can be updated dynamically."""
     def __init__(self, columnNameList, height=400, heightPolicy="auto", showLastRows=0, index_position=None):
         """@brief Constructor
            @param columnNameList A List of strings denoting each column in the 2 dimensional table.
            @param height The hieght of the table viewport in pixels.
            @param heightPolicy The height policy (auto, fixed, fit, min, max). default=fixed.
            @param showLastRows The number of rows to show in the table. If set to 2 then only
-                  the last two rows in the table are displayed but they ate scrolled into view. 
-                  The default=0 which will display all rows and will not scroll the latest 
+                  the last two rows in the table are displayed but they ate scrolled into view.
+                  The default=0 which will display all rows and will not scroll the latest
                   into view..
-           @param index_position The position of the index column in the table. 0 = the first 
+           @param index_position The position of the index column in the table. 0 = the first
                   column. Default is None which does not display the index column."""
         self._columnNameList = columnNameList
         self._dataDict = {}
         self._columns = []
         for columnName in columnNameList:
             self._dataDict[columnName]=[]
             self._columns.append( TableColumn(field=columnName, title=columnName) )
-            
+
         self._source = ColumnDataSource(self._dataDict)
 
         self._dataTable = DataTable(source=self._source, columns=self._columns, height=height, height_policy=heightPolicy, frozen_rows=-showLastRows, index_position=index_position)
-        
+
     def getWidget(self):
         """@brief return an instance of the table widget to be added to a layout."""
         return self._dataTable
-    
+
     def setRows(self, rowList):
         """@brief Set the rows in the table.
            @param rowList A list of rows of data. Each row must contain a list of values for each column in the table."""
         for row in rowList:
             if len(row) != len(self._columnNameList):
                 raise Exception("{} row should have {} values.".format(row, len(self._columnNameList)))
         dataDict = {}
         colIndex = 0
         for columnName in self._columnNameList:
             valueList = []
             for row in rowList:
                 valueList.append( row[colIndex] )
             dataDict[columnName]=valueList
-                
+
             colIndex = colIndex + 1
         self._source.data = dataDict
-        
+
     def appendRow(self, row):
         """@brief Set the rows in the table.
            @param rowList A list of rows of data. Each row must contain a list of values for each column in the table."""
         dataDict = {}
         colIndex = 0
         for columnName in self._columnNameList:
             valueList = [row[colIndex]]
-            dataDict[columnName]=valueList               
+            dataDict[columnName]=valueList
             colIndex = colIndex + 1
-        self._source.stream(dataDict) 
-    
+        self._source.stream(dataDict)
+
 class AlertButtonWrapper(object):
-    """@brief Responsible for presenting a button that when clicked displayed an alert dialog."""    
+    """@brief Responsible for presenting a button that when clicked displayed an alert dialog."""
     def __init__(self, buttonLabel, alertMessage, buttonType="default", onClickMethod=None):
         """@brief Constructor
-           @param buttonLabel The text displayed on the button. 
+           @param buttonLabel The text displayed on the button.
            @param alertMessage The message displayed in the alert dialog when clicked.
            @param buttonType The type of button to display (default, primary, success, warning, danger, light)).
-           @param onClickMethod An optional method that is called when the alert OK button has been clicked.  
+           @param onClickMethod An optional method that is called when the alert OK button has been clicked.
         """
         self._button = Button(label=buttonLabel, button_type=buttonType)
         if onClickMethod:
             self.addOnClickMethod(onClickMethod)
 
         source = {"msg": alertMessage}
         callback1 = CustomJS(args=dict(source=source), code="""
             var msg = source['msg']
             alert(msg);
         """)
         self._button.js_on_event(events.ButtonClick, callback1)
-        
+
     def addOnClickMethod(self, onClickMethod):
         """@brief Add a method that is called after the alert dialog has been displayed.
            @param onClickMethod The method that is called."""
-        self._button.on_click(onClickMethod)      
-        
+        self._button.on_click(onClickMethod)
+
     def getWidget(self):
         """@brief return an instance of the button widget to be added to a layout."""
         return self._button
-        
+
 class ShutdownButtonWrapper(object):
-    """@brief Responsible for presenting a shutdown button. When the button is clicked 
+    """@brief Responsible for presenting a shutdown button. When the button is clicked
               an alert message is displayed instructing the user to close the browser
               window. When the OK button in the alert dialog is clicked the
-              application is shutdown."""    
+              application is shutdown."""
     def __init__(self, shutDownMethod):
         """@brief Constructor
            @param shutDownMethod The method that is called to shutdown the application.
         """
         self._alertButtonWrapper = AlertButtonWrapper("Quit",\
                                                       "The application is shutting down. Please close the browser window",\
                                                       buttonType="danger",\
-                                                      onClickMethod=shutDownMethod)   
-        
+                                                      onClickMethod=shutDownMethod)
+
     def getWidget(self):
         """@brief return an instance of the shutdown button widget to be added to a layout."""
         return self._alertButtonWrapper.getWidget()
-    
-
```

### Comparing `p3lib-1.1.8/src/p3lib/boot_manager.py` & `p3lib-1.1.9/src/p3lib/boot_manager.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/database_if.py` & `p3lib-1.1.9/src/p3lib/database_if.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/helper.py` & `p3lib-1.1.9/src/p3lib/helper.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/json_networking.py` & `p3lib-1.1.9/src/p3lib/json_networking.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/mqtt_rpc.py` & `p3lib-1.1.9/src/p3lib/mqtt_rpc.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/netif.py` & `p3lib-1.1.9/src/p3lib/netif.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/netplotly.py` & `p3lib-1.1.9/src/p3lib/netplotly.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/pconfig.py` & `p3lib-1.1.9/src/p3lib/pconfig.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/ssh.py` & `p3lib-1.1.9/src/p3lib/ssh.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib/uio.py` & `p3lib-1.1.9/src/p3lib/uio.py`

 * *Files identical despite different names*

### Comparing `p3lib-1.1.8/src/p3lib.egg-info/PKG-INFO` & `p3lib-1.1.9/src/p3lib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p3lib
-Version: 1.1.8
+Version: 1.1.9
 Summary: A group of python modules for networking, plotting data, config storage, automating boot scripts, ssh access and user input output.
 Home-page: https://github.com/pjaos/p3lib
 Author: Paul Austen
 Author-email: pausten.os@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pjaos/p3lib/issues
 Platform: UNKNOWN
```

