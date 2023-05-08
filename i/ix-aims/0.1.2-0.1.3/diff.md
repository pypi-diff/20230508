# Comparing `tmp/ix_aims-0.1.2.tar.gz` & `tmp/ix_aims-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ix_aims-0.1.2.tar", max compression
+gzip compressed data, was "ix_aims-0.1.3.tar", max compression
```

## Comparing `ix_aims-0.1.2.tar` & `ix_aims-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.2/ix_aims/__init__.py
--rw-r--r--   0        0        0      606 2023-05-02 23:55:26.364346 ix_aims-0.1.2/ix_aims/cli.py
--rw-r--r--   0        0        0      212 2023-05-02 22:49:33.331758 ix_aims-0.1.2/ix_aims/imgs/__init__.py
--rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.2/ix_aims/imgs/plusTab.png
--rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.2/ix_aims/imgs/processesBtn.png
--rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.2/ix_aims/imgs/yesBtn.png
--rw-r--r--   0        0        0     3662 2023-05-02 23:06:56.142270 ix_aims-0.1.2/ix_aims/lib.py
--rw-r--r--   0        0        0      627 2023-05-02 23:54:22.328865 ix_aims-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 ix_aims-0.1.2/setup.py
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 ix_aims-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       18 2023-05-02 21:16:59.064713 ix_aims-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 21:33:19.881513 ix_aims-0.1.3/ix_aims/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-02 23:55:26.364346 ix_aims-0.1.3/ix_aims/cli.py
+-rw-r--r--   0        0        0      240 2023-05-03 17:44:05.589407 ix_aims-0.1.3/ix_aims/imgs/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-03 17:50:50.001156 ix_aims-0.1.3/ix_aims/imgs/ellipsBtn.png
+-rw-r--r--   0        0        0      322 2023-05-02 21:20:56.342365 ix_aims-0.1.3/ix_aims/imgs/plusTab.png
+-rw-r--r--   0        0        0     3615 2023-05-02 21:20:56.342365 ix_aims-0.1.3/ix_aims/imgs/processesBtn.png
+-rw-r--r--   0        0        0     2201 2023-05-02 21:20:56.342365 ix_aims-0.1.3/ix_aims/imgs/yesBtn.png
+-rw-r--r--   0        0        0     4513 2023-05-08 16:34:28.020924 ix_aims-0.1.3/ix_aims/lib.py
+-rw-r--r--   0        0        0      627 2023-05-08 16:34:45.528836 ix_aims-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 ix_aims-0.1.3/setup.py
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 ix_aims-0.1.3/PKG-INFO
```

### Comparing `ix_aims-0.1.2/ix_aims/cli.py` & `ix_aims-0.1.3/ix_aims/cli.py`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.2/ix_aims/imgs/processesBtn.png` & `ix_aims-0.1.3/ix_aims/imgs/processesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.2/ix_aims/imgs/yesBtn.png` & `ix_aims-0.1.3/ix_aims/imgs/yesBtn.png`

 * *Files identical despite different names*

### Comparing `ix_aims-0.1.2/ix_aims/lib.py` & `ix_aims-0.1.3/ix_aims/lib.py`

 * *Files 20% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     if res.status_code == 200:
         return res.json()
     else:
         res.raise_for_status()
 
 
-def setup_work_order_day(recipe_name, save_folder, rgb_params, nir_params):
+def setup_work_order_day(recipe_name, save_folder, rgb_params, nir_params, year, doy):
     # New Recipe
     click(imgs.plusTab)
     g.hotkey('tab')
     g.hotkey('ctrl', 'a')
     g.hotkey('del')
     g.typewrite(recipe_name)
 
@@ -119,18 +119,48 @@
         g.hotkey('del')
         g.typewrite(str(rgb_params[param]))
 
         g.hotkey('tab')
         g.hotkey('del')
         g.typewrite(str(nir_params[param]))
 
-    # # Select dirs
+    # Select dirs
     # g.hotkey('tab')
     # g.hotkey('tab')
     # g.hotkey('enter')
+    #
+    # # Find ellipses buttons
+    # sleep(1)
+    # buttons = list(map(g.center, g.locateAllOnScreen(imgs.ellipseBtn, confidence=.95)))
+    # assert len(buttons) == 2, "Could not find ellipses buttons"
+
+    # Select RGB images
+    #
+    # rgb_btn = min(buttons, key=lambda b: b.y)
+    # g.click(rgb_btn)
+
+    # for _ in range(7):
+    #     g.hotkey('tab')
+    # g.typewrite("aco-uvic")
+    # g.confirm("continue?")
+    # g.hotkey("enter")
+    # g.hotkey("tab")
+    # g.typewrite(f"{year}_Acquisitions")
+    # g.confirm("continue?")
+    # g.hotkey("enter")
+    # g.typewrite("01")
+    # g.hotkey("enter")
+    # g.typewrite(f"D{str(doy).zfill(3)}")
+    # g.confirm("continue?")
+    # g.hotkey("enter")
+
+    # nir_btn = max(buttons, key=lambda b: b.y)
+
+    # Click ellipses buttons
+
 
 
 def check_work_order_param(value: str):
     """Check worker order matches regex dd_dddd_dd pattern"""
     assert re.match(r'\d{2}_\d{4}_\d{2}',
                     value), "Work order must be in format dd_dddd_dd"
     return value
@@ -138,20 +168,21 @@
 
 def auto_ix(work_order: str):
     work_order = check_work_order_param(work_order)
     flights = get_acquisitions(work_order)
 
     # Open iXCapture
     # Use this if working in RDP client to activate the write window
+    # g.hotkey("ctrl", "alt", "right")
     # g.click(1000, 1000)
-    open_ix_capture()
-    sleep(10)
-    go_to_processes_tab()
-    sleep(2)
-    click_yes()
+    # open_ix_capture()
+    sleep(5)
+    # go_to_processes_tab()
+    # sleep(2)
+    # click_yes()
 
     for flight in flights:
         date = arrow.get(flight['acq_date'])
         sess = flight['sess_num']
         year = date.format('YYYY')
         doy = date.format('DDD')
 
@@ -159,8 +190,8 @@
         rgb_params = get_camera_params(date, "rgb")
 
         recipe_name = f"{work_order}_d{doy}"
         if sess:
             recipe_name += f"s{sess}"
         save_folder = f'C:\\CIR_files\\{year}'
 
-        setup_work_order_day(recipe_name, save_folder, rgb_params, nir_params)
+        setup_work_order_day(recipe_name, save_folder, rgb_params, nir_params, year, doy)
```

### Comparing `ix_aims-0.1.2/pyproject.toml` & `ix_aims-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ix-aims"
-version = "0.1.2"
+version = "0.1.3"
 description = "iX Capture automation with AIMS data"
 authors = ["Taylor Denouden <taylor.denouden@hakai.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "ix_aims"}]
 
 [tool.poetry.dependencies]
```

### Comparing `ix_aims-0.1.2/setup.py` & `ix_aims-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'typer>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['autoix = ix_aims.cli:main']}
 
 setup_kwargs = {
     'name': 'ix-aims',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'iX Capture automation with AIMS data',
     'long_description': '# auto-ix-capture\n',
     'author': 'Taylor Denouden',
     'author_email': 'taylor.denouden@hakai.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ix_aims-0.1.2/PKG-INFO` & `ix_aims-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ix-aims
-Version: 0.1.2
+Version: 0.1.3
 Summary: iX Capture automation with AIMS data
 License: MIT
 Author: Taylor Denouden
 Author-email: taylor.denouden@hakai.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

