# Comparing `tmp/streamlit-deckgl-0.2.0.tar.gz` & `tmp/streamlit-deckgl-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deckgl-0.2.0.tar", last modified: Fri May  5 06:22:19 2023, max compression
+gzip compressed data, was "streamlit-deckgl-0.2.1.tar", last modified: Mon May  8 19:48:16 2023, max compression
```

## Comparing `streamlit-deckgl-0.2.0.tar` & `streamlit-deckgl-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.939309 streamlit-deckgl-0.2.0/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1274 2023-04-28 04:00:31.000000 streamlit-deckgl-0.2.0/README.md
--rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-05 06:22:19.939309 streamlit-deckgl-0.2.0/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-05 06:11:32.000000 streamlit-deckgl-0.2.0/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.931309 streamlit-deckgl-0.2.0/src/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/src/streamlit_deckgl/
--rw-rw-r--   0 dave      (1000) dave      (1000)     2208 2023-05-05 06:11:18.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/
--rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/index.html
--rw-rw-r--   0 dave      (1000) dave      (1000)     2004 2023-05-05 05:17:15.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/main.js
--rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/style.css
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-05 06:22:19.935309 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1581 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-05 06:22:19.000000 streamlit-deckgl-0.2.0/src/streamlit_deckgl.egg-info/top_level.txt
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1066 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)       84 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2435 2023-05-08 19:47:36.000000 streamlit-deckgl-0.2.1/README.md
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)      718 2023-05-08 19:48:11.000000 streamlit-deckgl-0.2.1/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.130981 streamlit-deckgl-0.2.1/src/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.130981 streamlit-deckgl-0.2.1/src/streamlit_deckgl/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2188 2023-05-08 19:23:55.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.134981 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      770 2023-04-29 03:59:23.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/index.html
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2004 2023-05-05 05:17:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/main.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)   230931 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-04-28 00:01:01.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/style.css
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-08 19:48:16.130981 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2742 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      466 2023-05-08 19:48:16.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       34 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       17 2023-05-08 19:48:15.000000 streamlit-deckgl-0.2.1/src/streamlit_deckgl.egg-info/top_level.txt
```

### Comparing `streamlit-deckgl-0.2.0/LICENSE` & `streamlit-deckgl-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.2.0/PKG-INFO` & `streamlit-deckgl-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,52 @@
-Metadata-Version: 2.1
-Name: streamlit-deckgl
-Version: 0.2.0
-Summary: Streamlit component for deck.gl visualisation
-Author: Oceanum
-Author-email: developers@oceanum.science
-Keywords: streamlit,pydeck,deck.gl,visualisation
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # streamlit-deckgl
 
 Streamlit component for deck.gl visualisation with bi-directional transport for onClick events.
 
 ## Installation instructions
 
 ```sh
 pip install streamlit-deckgl
 ```
 
-## Usage instructions
+## Usage
+
+There is one component function `st_deckgl` with function signature:
+
+```
+component_value=st_deckgl(deck, height=500, configuration=None, key="deck_gl", events=None, description=None)
+```
+
+### Parameters
+
+    deck : pydeck.Deck instance
+        The pydeck map to render.
+    key : str, default "deck_gl"
+        The key for the component. This must be unique for each map in the app.
+    height : int, default 500
+        The height of the map in pixels.
+    events : list, default None
+        A dict of events to listen for. Can be one or more of:
+        - 'click'
+        - 'hover'
+        - 'drag'
+    description : dict, default None
+        A dictionary with additional description components to overlay on the map
+        The keys are the position which can be one of 'top-right','top-left','bottom-right','bottom-left'
+        The values are the html elements to place in each position
+        Example {'top-right':<div>This is a nice map</div>}
+    configuration : dict, default None
+        A dictionary of configuration options for the map.
+
+### Returns
+
+    component_value : dict
+        A dictionary containing the info dictionary of the event.
+
+## Example
 
 ```python
 import streamlit as st
 import pydeck as pdk
 import pandas as pd
 
 from streamlit_deckgl import st_deckgl
@@ -60,11 +83,11 @@
     ],
     tooltip={
         "html": "<b>Temperature:</b> {value} °C",
         "style": {"backgroundColor": "steelblue", "color": "white"},
     },
 )
 
-value = st_deckgl(r)
+value = st_deckgl(r,)
 
 st.write(value)
 ```
```

### Comparing `streamlit-deckgl-0.2.0/setup.py` & `streamlit-deckgl-0.2.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="streamlit-deckgl",
-    version="0.2.0",
+    version="0.2.1",
     author="Oceanum",
     author_email="developers@oceanum.science",
     description="Streamlit component for deck.gl visualisation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["streamlit_deckgl"],
     package_dir={"": "src"},
```

### Comparing `streamlit-deckgl-0.2.0/src/streamlit_deckgl/__init__.py` & `streamlit-deckgl-0.2.1/src/streamlit_deckgl/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,42 +12,42 @@
 _component_func = components.declare_component(
     "streamlit_deckgl", path=str(frontend_dir)
 )
 
 # Create the python function that will be called
 def st_deckgl(
     deck: pdk.Deck,
-    height: int = 500,
-    configuration: Optional[dict] = None,
     key: Optional[str] = "deck_gl",
+    height: int = 500,
     events: Optional[list] = None,
     description: Optional[dict] = None,
+    configuration: Optional[dict] = None,
 ):
     """Create a deck.gl map in Streamlit.
 
     Parameters
     ==========
     deck : pydeck.Deck instance
         The pydeck map to render.
-    height : int, default 500
-        The height of the map in pixels.
-    configuration : dict, default None
-        A dictionary of configuration options for the map.
     key : str, default "deck_gl"
         The key for the component. This must be unique for each map in the app.
-    events : list, default ['click','hover','drag']
+    height : int, default 500
+        The height of the map in pixels.
+    events : list, default None
         A dict of events to listen for. Can be one or more of:
         - 'click'
         - 'hover'
         - 'drag'
     description : dict, default None
         A dictionary with additional description components to overlay on the map
         The keys are the position which can be one of 'top-right','top-left','bottom-right','bottom-left'
         The values are the html elements to place in each position
         Example {'top-right':<div>This is a nice map</div>}
+    configuration : dict, default None
+        A dictionary of configuration options for the map.
 
     Returns
     =======
     component_value : dict
         A dictionary containing the info dictionary of the event.
 
     """
```

### Comparing `streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/index.html` & `streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/index.html`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/main.js` & `streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/main.js`

 * *Files identical despite different names*

### Comparing `streamlit-deckgl-0.2.0/src/streamlit_deckgl/frontend/streamlit-component-lib.js` & `streamlit-deckgl-0.2.1/src/streamlit_deckgl/frontend/streamlit-component-lib.js`

 * *Files identical despite different names*

