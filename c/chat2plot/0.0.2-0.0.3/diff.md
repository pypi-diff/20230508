# Comparing `tmp/chat2plot-0.0.2.tar.gz` & `tmp/chat2plot-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat2plot-0.0.2.tar", last modified: Sun May  7 15:17:36 2023, max compression
+gzip compressed data, was "chat2plot-0.0.3.tar", last modified: Mon May  8 16:23:30 2023, max compression
```

## Comparing `chat2plot-0.0.2.tar` & `chat2plot-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:36.426111 chat2plot-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-07 15:17:25.000000 chat2plot-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 15:17:25.000000 chat2plot-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-07 15:17:36.426111 chat2plot-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-07 15:17:25.000000 chat2plot-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:36.426111 chat2plot-0.0.2/chat2plot/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9223 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/chat2plot.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/dataset_description.py
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/render.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 15:17:25.000000 chat2plot-0.0.2/chat2plot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 15:17:36.426111 chat2plot-0.0.2/chat2plot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 15:17:36.000000 chat2plot-0.0.2/chat2plot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-07 15:17:25.000000 chat2plot-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-07 15:17:25.000000 chat2plot-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-07 15:17:36.426111 chat2plot-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-07 15:17:25.000000 chat2plot-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:23:30.321515 chat2plot-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-08 16:23:19.000000 chat2plot-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 16:23:19.000000 chat2plot-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-08 16:23:30.321515 chat2plot-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-08 16:23:19.000000 chat2plot-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:23:30.321515 chat2plot-0.0.3/chat2plot/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10962 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/chat2plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/dataset_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4367 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 16:23:19.000000 chat2plot-0.0.3/chat2plot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 16:23:30.321515 chat2plot-0.0.3/chat2plot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-08 16:23:30.000000 chat2plot-0.0.3/chat2plot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-08 16:23:30.000000 chat2plot-0.0.3/chat2plot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 16:23:30.000000 chat2plot-0.0.3/chat2plot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 16:23:30.000000 chat2plot-0.0.3/chat2plot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 16:23:30.000000 chat2plot-0.0.3/chat2plot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-08 16:23:19.000000 chat2plot-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-08 16:23:19.000000 chat2plot-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-08 16:23:30.325516 chat2plot-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-08 16:23:19.000000 chat2plot-0.0.3/setup.py
```

### Comparing `chat2plot-0.0.2/LICENSE` & `chat2plot-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.2/PKG-INFO` & `chat2plot-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat2plot
-Version: 0.0.2
+Version: 0.0.3
 Summary: chat to visualization with LLM
 Home-page: https://github.com/nyanp/chat2plot
 Author: nyanp
 Author-email: Noumi.Taiga@gmail.com
 License: MIT
 Keywords: llm visualization chart gpt
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📈 Chat2Plot - interactive text-to-visualization with LLM
 
 Chat2plot is a project that provides visualizations based on chat instructions for given data.
 
+demo: https://chat2plot-sample.streamlit.app/
+
 ## Usage
 
 ```Python
 import os
 import pandas as pd
 from chat2plot import chat2plot
 
@@ -33,30 +35,39 @@
 c2p = chat2plot(df)
 
 # 3. Plot chart interactively
 c2p("average target over countries")
 
 c2p("change to horizontal-bar chart")
 
-cp2("...")
+c2p("...")
 ```
 
 ## Why Chat2Plpot
 
-Inside Chat2Plot, LLM does not generate Python code, but rather a declarative data structure representing the plot specification.
+Inside Chat2Plot, LLM does not generate Python code,
+but generates plot specifications in json.
+
+The declarative visualization specification in json is transformed into actual charts in 
+Chat2Plot using plotly or altair, but users can also use json directly in their own applications.
 
-While this design has a lower capacity of plots that can be generated compared to Python code (e.g., ChatGPT's Code Interpreter Plugin), it has the following practical advantages:
+This design limits the visualization expression compared to Python code generation 
+(such as ChatGPT's Code Interpreter Plugin), but has the following practical advantages:
 
 - Secure
     - More secure execution, as LLM does not directly generate code.
 
 - Language-independent
-    - Declarative data structures are language-independent, making it easy to plot in non-Python environments.
+    - Declarative data structures are language-agnostic, making it easy to plot in non-Python environments.
 
 - Interactive
     - Declarative data can be modified by the user to improve plots through collaborative work between the user and LLM.
 
-This declarative data structure can be chosen between default (simple dataclass) and the vega-lite format.
+The json schema can be selected from a default simple definition or a vega-lite compliant schema.
 
 ```Python
 c2p = chat2plot(df, "vega")  # use vega-lite format
+
+ret = c2p("plot x vs y")
+
+ret.config  # get vega-lite compliant json data
 ```
```

### Comparing `chat2plot-0.0.2/README.md` & `chat2plot-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # 📈 Chat2Plot - interactive text-to-visualization with LLM
 
 Chat2plot is a project that provides visualizations based on chat instructions for given data.
 
+demo: https://chat2plot-sample.streamlit.app/
+
 ## Usage
 
 ```Python
 import os
 import pandas as pd
 from chat2plot import chat2plot
 
@@ -18,30 +20,39 @@
 c2p = chat2plot(df)
 
 # 3. Plot chart interactively
 c2p("average target over countries")
 
 c2p("change to horizontal-bar chart")
 
-cp2("...")
+c2p("...")
 ```
 
 ## Why Chat2Plpot
 
-Inside Chat2Plot, LLM does not generate Python code, but rather a declarative data structure representing the plot specification.
+Inside Chat2Plot, LLM does not generate Python code,
+but generates plot specifications in json.
+
+The declarative visualization specification in json is transformed into actual charts in 
+Chat2Plot using plotly or altair, but users can also use json directly in their own applications.
 
-While this design has a lower capacity of plots that can be generated compared to Python code (e.g., ChatGPT's Code Interpreter Plugin), it has the following practical advantages:
+This design limits the visualization expression compared to Python code generation 
+(such as ChatGPT's Code Interpreter Plugin), but has the following practical advantages:
 
 - Secure
     - More secure execution, as LLM does not directly generate code.
 
 - Language-independent
-    - Declarative data structures are language-independent, making it easy to plot in non-Python environments.
+    - Declarative data structures are language-agnostic, making it easy to plot in non-Python environments.
 
 - Interactive
     - Declarative data can be modified by the user to improve plots through collaborative work between the user and LLM.
 
-This declarative data structure can be chosen between default (simple dataclass) and the vega-lite format.
+The json schema can be selected from a default simple definition or a vega-lite compliant schema.
 
 ```Python
 c2p = chat2plot(df, "vega")  # use vega-lite format
+
+ret = c2p("plot x vs y")
+
+ret.config  # get vega-lite compliant json data
 ```
```

### Comparing `chat2plot-0.0.2/chat2plot/chat2plot.py` & `chat2plot-0.0.3/chat2plot/chat2plot.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,58 +17,160 @@
 from chat2plot.schema import LLMResponse, PlotConfig, ResponseType
 
 _logger = getLogger(__name__)
 
 _PROMPT = """
 Your task is to generate chart configuration for the given dataset and user question delimited by <>.
 
-Responses should be in JSON format including the following keys:
+Responses should be in JSON format compliant to the following JSON Schema.
 
-chart_type: the type of chart, should be one of [line, scatter, bar, pie, horizontal-bar, area]
-measures: list of measure, which each measure shoule be expressed as the combination of aggregations (should be one of [SUM, AVG, COUNT, MAX, MIN, DISTINCT_COUNT]) and column (should be numeric), like "SUM(price)". If the chart is a scatter plot, aggregation should be omitted and simply answer the column name. The length of the list is 2 only for scatter plot and 1 otherwise.
-dimension: group-by column, which should be categorical/datetime variables used as axis.
-filters: list of filter conditions, where each filter must be in a valid format as an argument to the pandas df.query() method.
-hue: (optional) dimension used as grouping variables that will produce different colors.
-xmin: (optional) minimum value of x-axis.
-xmax: (optional) maximum value of x-axis.
-ymin: (optional) minimum value of y-axis.
-ymax: (optional) maximum value of y-axis.
-xlabel: (optional) label of x-axis.
-ylabel: (optional) label of y-axis.
-sort_criteria: (optional) the sorting criteria for x-axis, should be one of [name, value].
-sort_order: (optional) sorting order, should be one of [asc, desc].
+{{
+  "title": "Chart config",
+  "description": "A configuration of chart",
+  "type": "object",
+  "properties": {{
+    "chart_type": {{
+      "description": "the type of the chart",
+      "type": "string",
+      "enum": [
+        "line",
+        "scatter",
+        "bar",
+        "pie",
+        "horizontal-bar",
+        "area"
+      ]
+    }},
+    "x": {{
+      "description": "X-axis column for the chart, or label column for pie chart.",
+      "type": "object",
+      "properties": {{
+        "column": {{
+          "description": "Column name of the dataset used as x-axis",
+          "type": "string"
+        }}
+      }},
+      "required": ["column"]
+    }},
+    "y": {{
+      "description": "Y-axis column for the chart, or value column for pie chart.",
+      "type": "object",
+      "properties": {{
+        "column": {{
+          "description": "Column name of the dataset used as y-axis",
+          "type": "string"
+        }},
+        "aggregation": {{
+          "description": "Type of aggregation. will be ignored when it is scatter plot.
+          "type": "string",
+          "enum": [
+            "SUM",
+            "AVG",
+            "COUNT",
+            "MAX",
+            "MIN",
+            "DISTINCT_COUNT"
+          ]
+        }}
+      }},
+      "required": ["column"]
+    }},
+    "filters": {{
+      "description": "List of filter conditions, where each filter must be in a valid format as an argument to the pandas df.query() method.",
+      "type": "array",
+      "items": {{
+        "type": "string"
+      }}
+    }},
+    "hue": {{
+      "description": "Dimension used as grouping variables that will produce different colors.",
+      "type": "object",
+      "properties": {{
+        "column": {{
+          "type": "string"
+        }}
+      }},
+      "required": ["column"]
+    }},
+    "xmin": {{
+      "description": "Minimum value of x-axis",
+      "type": "number"
+    }},
+    "xmax": {{
+      "description": "Maximum value of x-axis",
+      "type": "number"
+    }},
+    "ymin": {{
+      "description": "Minimum value of y-axis",
+      "type": "number"
+    }},
+    "ymax": {{
+      "description": "Maximum value of y-axis",
+      "type": "number"
+    }},
+    "xlabel": {{
+      "description": "Label of x-axis",
+      "type": "string"
+    }},
+    "ylabel": {{
+      "description": "Label of y-axis",
+      "type": "string"
+    }},
+    "sort_criteria": {{
+      "description": "The sorting criteria for x-axis",
+      "type": "string",
+      "enum": [
+        "name",
+        "value"
+      ]
+    }},
+    "sort_order": {{
+      "description": "Sorting order for x-axis",
+      "type": "string",
+      "enum": [
+        "asc",
+        "desc"
+      ]
+    }},
+  }},
+  "required": [
+    "chart_type",
+    "y"
+  ]
+}}
 
-If a transform is needed for a column used for a measure or dimension, one of the following transform functions can be used instead of specifying the column directly.
+Instead of specifying column names in the dataset directly for `x.column` and `y.column`, you can use one of the following conversion functions if necessary:
 
 BINNING(column, interval): binning a numerical column to the specified interval. interval should be integer literal. example: BINNING(x, 10)
 ROUND_DATETIME(column, period): binning a date/datetime column to the specified period. period should be one of [day, week, month, year]. example: ROUND_DATETIME(x, year)
 
 The user's question may be an instruction to fine-tune the previous chart, or it may be an instruction to create a new chart based on a completely new context. In the latter case, be careful not to use the context used for the previous chart.
 
 If the user's question does not fall under any of above keys and is not a request about the appearance of the chart, simply reply "not related".
 
-Dataset contains the following contents:
+This is the result of `print(df.head())`:
 
 {dataset}
 
-The output json must be enclosed in triple brackets.
+Make sure to prefix the requested json string with triple backticks exactly and suffix the json with triple backticks exactly.
 """
 
+
 _PROMPT_VEGA = """
 Your task is to generate chart configuration for the given dataset and user question delimited by <>.
 
 Responses should be in JSON format compliant with the vega-lite specification, but `data` field must be excluded.
 
 If the user's question does not fall under any of above keys and is not a request about the appearance of the chart, simply reply "not related".
 
-Dataset contains the following contents:
+This is the result of `print(df.head())`:
 
 {dataset}
 
-The output json must be enclosed in triple brackets.
+Make sure to prefix the requested json string with triple backticks exactly and suffix the json with triple backticks exactly.
 """
 
 
 @dataclass(frozen=True)
 class Plot:
     figure: alt.Chart | Figure | None
     config: PlotConfig | dict[str, Any] | None
@@ -126,15 +228,15 @@
         return self.query(q, show_plot)
 
 
 class Chat2Plot(Chat2PlotBase):
     def __init__(
         self, df: pd.DataFrame, chat: BaseChatModel | None = None, verbose: bool = False
     ):
-        self._session = ChatSession(df, _PROMPT, "User Question: <{text}>", chat)
+        self._session = ChatSession(df, _PROMPT, "<{text}>", chat)
         self._df = df
         self._verbose = verbose
 
     @property
     def session(self) -> ChatSession:
         return self._session
 
@@ -180,15 +282,15 @@
             return LLMResponse(ResponseType.UNKNOWN)
 
 
 class Chat2Vega(Chat2PlotBase):
     def __init__(
         self, df: pd.DataFrame, chat: BaseChatModel | None = None, verbose: bool = False
     ):
-        self._session = ChatSession(df, _PROMPT_VEGA, "User Question: <{text}>", chat)
+        self._session = ChatSession(df, _PROMPT_VEGA, "<{text}>", chat)
         self._df = df
         self._verbose = verbose
 
     @property
     def session(self) -> ChatSession:
         return self._session
 
@@ -235,11 +337,12 @@
         )
 
 
 def parse_json(content: str) -> dict[str, Any]:
     try:
         return json.loads(content)  # type: ignore
     except ValueError:
-        s = re.search(r"```(.*)```", content, re.MULTILINE | re.DOTALL)
+        ptn = r"```json(.*)```" if "```json" in content else r"```(.*)```"
+        s = re.search(ptn, content, re.MULTILINE | re.DOTALL)
         if s:
             return json.loads(s.group(1))  # type: ignore
         raise
```

### Comparing `chat2plot-0.0.2/chat2plot/render.py` & `chat2plot-0.0.3/chat2plot/render.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import copy
 from typing import Any
 
 import altair as alt
 import pandas as pd
 import plotly.express as px
+import vegafusion as vf
 from altair.utils.data import to_values
 from plotly.graph_objs import Figure
 
 from chat2plot.schema import (
     AggregationType,
     ChartType,
     Filter,
@@ -31,15 +32,15 @@
         ax["labels"] = labels
 
     return ax
 
 
 def draw_plotly(df: pd.DataFrame, config: PlotConfig, show: bool = True) -> Figure:
     df_filtered = filter_data(df, config.filters).copy()
-    df_filtered = transform(df, config)
+    df_filtered = transform(df_filtered, config)
 
     chart_type = config.chart_type
 
     if chart_type in [ChartType.BAR, ChartType.HORIZONTAL_BAR]:
         agg = groupby_agg(df_filtered, config)
         x = agg.columns[0]
         y = agg.columns[-1]
@@ -52,103 +53,101 @@
         fig = px.bar(
             agg,
             color=config.hue.column if config.hue else None,
             orientation=orientation,
             **_ax_config(config, x, y),
         )
     elif chart_type == ChartType.SCATTER:
+        assert config.x is not None
         fig = px.scatter(
             df_filtered,
             color=config.hue.column if config.hue else None,
-            **_ax_config(config, config.measures[0].column, config.measures[1].column),
+            **_ax_config(config, config.x.column, config.y.column),
         )
     elif chart_type == ChartType.PIE:
         agg = groupby_agg(df_filtered, config)
         fig = px.pie(agg, names=agg.columns[0], values=agg.columns[-1])
     elif chart_type in [ChartType.LINE, ChartType.AREA]:
         func_table = {ChartType.LINE: px.line, ChartType.AREA: px.area}
 
         if is_aggregation(config):
             agg = groupby_agg(df_filtered, config)
             fig = func_table[chart_type](
                 agg, **_ax_config(config, agg.columns[0], y=agg.columns[-1])
             )
         else:
-            assert config.dimension is not None
+            assert config.x is not None
             fig = func_table[chart_type](
                 df_filtered,
                 color=config.hue.column if config.hue else None,
-                **_ax_config(
-                    config, config.dimension.column, config.measures[0].column
-                ),
+                **_ax_config(config, config.x.column, config.y.column),
             )
     else:
         raise ValueError(f"Unknown chart_type: {chart_type}")
 
     if show:
         fig.show()
 
     return fig
 
 
 def draw_altair(
-    df: pd.DataFrame, config: dict[str, Any], show: bool = True
+    df: pd.DataFrame,
+    config: dict[str, Any],
+    show: bool = True,
+    use_vega_fusion: bool = True,
 ) -> alt.Chart:
+    if use_vega_fusion:
+        vf.enable()
     spec = copy.deepcopy(config)
     spec["data"] = to_values(df)
     chart = alt.Chart.from_dict(spec)
     if show:
         chart.show()
 
     return chart
 
 
 def groupby_agg(df: pd.DataFrame, config: PlotConfig) -> pd.DataFrame:
-    assert len(config.measures) == 1
+    group_by = [config.x.column] if config.x is not None else []
 
-    group_by = [config.dimension.column] if config.dimension is not None else []
-
-    if config.hue and config.hue != config.dimension:
+    if config.hue and config.hue != config.x:
         group_by.append(config.hue.column)
 
     agg_method = {
         AggregationType.AVG: "mean",
         AggregationType.SUM: "sum",
         AggregationType.COUNT: "count",
         AggregationType.DISTINCT_COUNT: "nunique",
         AggregationType.MIN: "min",
         AggregationType.MAX: "max",
     }
 
-    m = config.measures[0]
-    assert m.aggregation_method is not None
+    m = config.y
+    assert m.aggregation is not None
 
     if not group_by:
-        return pd.DataFrame(
-            {str(m): [df[m.column].agg(agg_method[m.aggregation_method])]}
-        )
+        return pd.DataFrame({str(m): [df[m.column].agg(agg_method[m.aggregation])]})
     else:
         agg = (
             df.groupby(group_by, dropna=False)[m.column]
-            .agg(agg_method[m.aggregation_method])
+            .agg(agg_method[m.aggregation])
             .rename(str(m))
         )
         ascending = config.sort_order == SortOrder.ASC
 
         if config.sort_criteria == SortingCriteria.NAME:
             agg = agg.sort_index(ascending=ascending)
         elif config.sort_criteria == SortingCriteria.VALUE:
             agg = agg.sort_values(ascending=ascending)
 
         return agg.reset_index()
 
 
 def is_aggregation(config: PlotConfig) -> bool:
-    return (
-        len(config.measures) == 1 and config.measures[0].aggregation_method is not None
-    )
+    return config.y.aggregation is not None
 
 
 def filter_data(df: pd.DataFrame, filters: list[Filter]) -> pd.DataFrame:
     if not filters:
         return df
     return df.query(" and ".join([f.query for f in filters]))
```

### Comparing `chat2plot-0.0.2/chat2plot/schema.py` & `chat2plot-0.0.3/chat2plot/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import re
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any
 
 
-class ChartType(Enum):
+class ChartType(str, Enum):
     PIE = "pie"
     SCATTER = "scatter"
     LINE = "line"
     BAR = "bar"
     AREA = "area"
     HORIZONTAL_BAR = "horizontal-bar"
 
 
-class AggregationType(Enum):
+class AggregationType(str, Enum):
     SUM = "SUM"
     AVG = "AVG"
     MIN = "MIN"
     MAX = "MAX"
     COUNT = "COUNT"
     DISTINCT_COUNT = "DISTINCT_COUNT"
 
 
-class ResponseType(Enum):
+class ResponseType(str, Enum):
     SUCCESS = "success"
     NOT_RELATED = "not related"
     UNKNOWN = "unknown"
     FAILED_TO_RENDER = "failed to render"
 
 
-class SortingCriteria(Enum):
+class SortingCriteria(str, Enum):
     NAME = "name"
     VALUE = "value"
 
 
-class SortOrder(Enum):
+class SortOrder(str, Enum):
     ASC = "asc"
     DESC = "desc"
 
 
 @dataclass(frozen=True)
 class Measure:
     column: str
@@ -57,73 +57,75 @@
         if self.aggregation_method:
             return f"{self.aggregation_method.value}({self.column})"
         else:
             return self.column
 
 
 @dataclass(frozen=True)
-class Dimension:
+class Field:
     column: str
+    aggregation: AggregationType | None = None
+
+    @classmethod
+    def from_dict(cls, d: dict[str, str]) -> "Field":
+        return Field(
+            d["column"],
+            AggregationType(d["aggregation"]) if d.get("aggregation") else None,
+        )
 
 
 @dataclass(frozen=True)
 class Filter:
     query: str
 
 
 @dataclass
 class PlotConfig:
     chart_type: ChartType
-    measures: list[Measure]
-    dimension: Dimension | None
+    x: Field | None
+    y: Field
     filters: list[Filter]
-    hue: Dimension | None = None
+    hue: Field | None = None
     xmin: float | None = None
     xmax: float | None = None
     ymin: float | None = None
     ymax: float | None = None
     xlabel: str | None = None
     ylabel: str | None = None
     sort_criteria: SortingCriteria | None = None
     sort_order: SortOrder | None = None
 
     @property
     def required_columns(self) -> list[str]:
-        columns = [m.column for m in self.measures]
-        if self.dimension:
-            columns.append(self.dimension.column)
+        columns = [self.y.column]
+        if self.x:
+            columns.append(self.x.column)
         return columns
 
     @classmethod
     def from_json(cls, json_data: dict[str, Any]) -> "PlotConfig":
         assert "chart_type" in json_data
-        assert "dimension" in json_data
+        assert "y" in json_data
 
         def wrap_if_not_list(value: str | list[str]) -> list[str]:
             if not isinstance(value, list):
-                return [] if value is None else [value]
+                return [] if not value else [value]
             else:
                 return value
 
         chart_type = ChartType(json_data["chart_type"])
-        measures = [
-            Measure.from_text(m)
-            for m in wrap_if_not_list(json_data.get("measures", []))
-        ]
-        dimension = (
-            Dimension(json_data["dimension"]) if json_data.get("dimension") else None
-        )
+
         filters = [Filter(q) for q in wrap_if_not_list(json_data.get("filters", []))]
 
         return cls(
             chart_type,
-            measures,
-            dimension,
+            Field.from_dict(json_data["x"]) if json_data.get("x") else None,
+            Field.from_dict(json_data["y"]),
             filters,
-            Dimension(json_data["hue"]) if json_data.get("hue") else None,
+            Field.from_dict(json_data["hue"]) if json_data.get("hue") else None,
             json_data.get("xmin"),
             json_data.get("xmax"),
             json_data.get("ymin"),
             json_data.get("ymax"),
             json_data.get("xlabel"),
             json_data.get("ylabel"),
             SortingCriteria(json_data["sort_criteria"])
```

### Comparing `chat2plot-0.0.2/chat2plot/transform.py` & `chat2plot-0.0.3/chat2plot/transform.py`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.2/chat2plot.egg-info/PKG-INFO` & `chat2plot-0.0.3/chat2plot.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat2plot
-Version: 0.0.2
+Version: 0.0.3
 Summary: chat to visualization with LLM
 Home-page: https://github.com/nyanp/chat2plot
 Author: nyanp
 Author-email: Noumi.Taiga@gmail.com
 License: MIT
 Keywords: llm visualization chart gpt
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 📈 Chat2Plot - interactive text-to-visualization with LLM
 
 Chat2plot is a project that provides visualizations based on chat instructions for given data.
 
+demo: https://chat2plot-sample.streamlit.app/
+
 ## Usage
 
 ```Python
 import os
 import pandas as pd
 from chat2plot import chat2plot
 
@@ -33,30 +35,39 @@
 c2p = chat2plot(df)
 
 # 3. Plot chart interactively
 c2p("average target over countries")
 
 c2p("change to horizontal-bar chart")
 
-cp2("...")
+c2p("...")
 ```
 
 ## Why Chat2Plpot
 
-Inside Chat2Plot, LLM does not generate Python code, but rather a declarative data structure representing the plot specification.
+Inside Chat2Plot, LLM does not generate Python code,
+but generates plot specifications in json.
+
+The declarative visualization specification in json is transformed into actual charts in 
+Chat2Plot using plotly or altair, but users can also use json directly in their own applications.
 
-While this design has a lower capacity of plots that can be generated compared to Python code (e.g., ChatGPT's Code Interpreter Plugin), it has the following practical advantages:
+This design limits the visualization expression compared to Python code generation 
+(such as ChatGPT's Code Interpreter Plugin), but has the following practical advantages:
 
 - Secure
     - More secure execution, as LLM does not directly generate code.
 
 - Language-independent
-    - Declarative data structures are language-independent, making it easy to plot in non-Python environments.
+    - Declarative data structures are language-agnostic, making it easy to plot in non-Python environments.
 
 - Interactive
     - Declarative data can be modified by the user to improve plots through collaborative work between the user and LLM.
 
-This declarative data structure can be chosen between default (simple dataclass) and the vega-lite format.
+The json schema can be selected from a default simple definition or a vega-lite compliant schema.
 
 ```Python
 c2p = chat2plot(df, "vega")  # use vega-lite format
+
+ret = c2p("plot x vs y")
+
+ret.config  # get vega-lite compliant json data
 ```
```

### Comparing `chat2plot-0.0.2/setup.cfg` & `chat2plot-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `chat2plot-0.0.2/setup.py` & `chat2plot-0.0.3/setup.py`

 * *Files identical despite different names*

